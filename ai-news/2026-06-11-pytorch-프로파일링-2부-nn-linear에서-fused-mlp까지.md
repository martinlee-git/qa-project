# PyTorch 프로파일링(2부): nn.Linear에서 Fused MLP까지
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/torch-mlp-fusion
- Published At: Thu, 11 Jun 2026 00:00:00 GMT
- Collected At: 2026-06-11T20:48:46.842Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-PyTorch-2-nn-Linear-Fused-MLP-37cfc93aec5781138de0dbcbd8906cec
- Original Title: Profiling in PyTorch (Part 2): From nn.Linear to a Fused MLP
## Summary
우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다. matmul-add에서 Linear까지 전치(transpose)는 무엇을 하고 있나요? mul</code> 및 <code>add</code> 커널?"> 별도의 mul 및 추가 커널이 없는 이유는 무엇입니까? --compile이 단일 선형에 도움이 될 수 있습니까? 전치(transpose)는 어디로 갔습니까? 커널 레이아웃 및 pre-ops 세 개의 선형 쌓기: MLP 두 가지 유형의 GEMM 커널이 있는 이유는 무엇입니까? torch.compile</code>은 무엇을 합니까?"> torch.compile은 무엇을 합니까? 융합된 Triton 커널 손으로 조정한 커널을 사용하자 커널 라이브러리를 사용하는 이유 조정된 커널이 더 나은 이유 결론 이 시리즈 "PyTorch에서 프로파일링"의 첫 번째 부분에서 우리는 torch.add(torch.matmul(x, w), b)를 사용하여 학습했습니다…

## Original Description

We’re on a journey to advance and democratize artificial intelligence through open source and open science.
## Key Points
- 우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다.
- matmul-add에서 Linear까지 전치(transpose)는 무엇을 하고 있나요?
- mul</code> 및 <code>add</code> 커널?"> 왜 별도의 mul 및 add 커널이 없나요?
## Excerpt
matmul-add에서 Linear까지 전치(transpose)는 무엇을 하고 있나요? mul</code> 및 <code>add</code> 커널?"> 별도의 mul 및 추가 커널이 없는 이유는 무엇입니까? --compile이 단일 선형에 도움이 될 수 있습니까? 전치(transpose)는 어디로 갔습니까? 커널 레이아웃 및 pre-ops 세 개의 선형 쌓기: MLP 두 가지 유형의 GEMM 커널이 있는 이유는 무엇입니까? torch.compile</code>은 무엇을 합니까?"> torch.compile은 무엇을 합니까? 융합된 Triton 커널 수동으로 조정된 커널을 사용하자 커널 라이브러리를 사용하는 이유 조정된 커널이 더 나은 이유 결론 이 시리즈 "PyTorch에서 프로파일링"의 첫 번째 부분에서는 torch.add(torch.matmul(x, w), b)를 사용하여 PyTorch 프로파일러 추적을 읽는 방법을 배웠습니다. 우리는 또한 CPU 디스패치 체인, 실행 오버헤드, 오버헤드 바인딩과 컴퓨팅 바인딩 체제의 차이점, torch.compile의 일부 내부 등 여러 다른 주제에 대해서도 논의했습니다. 두 번째 반복(이 블로그 게시물)에서는 사다리를 한 단계 위로 올라갑니다. 손으로 작성한 matmul-add 쌍을 nn.Linear(bias=True 포함)로 대체합니다. 이는 모든 딥 러닝 모델이 사용하는 구성 요소입니다. 그런 다음 그 중 3개(우리 예에 해당)를 중간에 활성화하여 쌓아서 MLP(Multilayer Perceptron) 블록을 형성합니다. 이 블로그 게시물의 스크립트는 02_linear.py , 03_simple_mlp.py 및 03_kernels_mlp.py 에 있습니다. 이전과 마찬가지로 별도의 탭에서 열고 읽으면서 코드를 살펴보는 것이 도움이 됩니다. NVIDIA A100-SXM4-80GB GPU를 사용하여 스크립트를 실행합니다. Hugging Face 인프라에 GPU를 설정하는 것은 정말 쉽습니다.Spaces와 함께 Dev Mode를 사용하여 스크립트를 실험해 보세요. Hugging Face Jobs 파이프라인을 사용하여 스크립트를 실행할 수도 있습니다. 시작하기 전에 우리가 반복해서 의지할 두 가지 아이디어를 간단히 요약해 보겠습니다.