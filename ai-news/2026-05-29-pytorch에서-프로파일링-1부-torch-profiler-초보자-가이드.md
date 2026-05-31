# PyTorch에서 프로파일링(1부): torch.profiler 초보자 가이드
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/torch-profiler
- Published At: Fri, 29 May 2026 00:00:00 GMT
- Collected At: 2026-05-31T22:49:56.657Z
- Notion Page: https://www.notion.so/Hugging-Face-Blog-PyTorch-1-torch-profiler-36ffc93aec578124ae7cd6352d3f0eea
- Original Title: Profiling in PyTorch (Part 1): A Beginner&apos;s Guide to torch.profiler
## Summary
우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다. 행렬 곱셈 및 덧셈 연산 64x64 추적 ProfilerStep#2가 왜 그렇게 오래 걸립니까? CPU와 GPU 레인 사이에 ~2.5ms의 오프셋이 있는 이유는 무엇입니까? 이벤트 체인 matmul에 추가 CUDA 런타임 호출이 있는 이유는 무엇입니까? cudaDeviceSynchronize가 왜 그렇게 큰가요(~1.78ms)? 4096x4096 트레이스 동일한 커널이 다른 커널에 비해 시간이 더 오래 걸리는 이유는 무엇입니까? 작업 중인 토치 컴파일을 살펴보겠습니다. matmul을 융합하고 커널을 하나로 추가했습니까? torch.compile의 런타임 아키텍처 CUDA 실행이 절반으로 줄어들나요? CPU 오버헤드는 감소하지 않고 증가했습니다. 추적 읽기 치트시트 Profiler ta…

## Original Description

We’re on a journey to advance and democratize artificial intelligence through open source and open science.
## Key Points
- 우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다.
- 행렬 곱셈 및 덧셈 연산 64x64 추적 ProfilerStep#2가 왜 그렇게 오래 걸립니까?
- CPU와 GPU 레인 사이에 ~2.5ms의 오프셋이 있는 이유는 무엇입니까?
## Excerpt
행렬 곱셈 및 덧셈 연산 64x64 추적 ProfilerStep#2가 왜 그렇게 오래 걸립니까? CPU와 GPU 레인 사이에 ~2.5ms의 오프셋이 있는 이유는 무엇입니까? 이벤트 체인 matmul에 추가 CUDA 런타임 호출이 있는 이유는 무엇입니까? cudaDeviceSynchronize가 왜 그렇게 큰가요(~1.78ms)? 4096x4096 트레이스 동일한 커널이 다른 커널에 비해 시간이 더 오래 걸리는 이유는 무엇입니까? 작업 중인 토치 컴파일을 살펴보겠습니다. matmul을 융합하고 커널을 하나로 추가했습니까? torch.compile의 런타임 아키텍처 CUDA 실행이 절반으로 줄어들나요? CPU 오버헤드가 감소하지 않고 증가했습니다 추적 읽기 치트시트 프로파일러 테이블 CPU 레인 GPU 레인 디스패치 체인 torch.compile 결론 프로파일링할 수 없는 것은 최적화할 수 없습니다. LLM(대형 언어 모델)에서 초당 더 많은 토큰을 짜내려고 하거나, 추론에서 밀리초를 줄이려고 하거나, 훈련 루프가 사양 시트에서 약속한 것보다 느리게 실행되는 이유를 이해하려는 경우 경로는 결국 프로파일링을 통해 실행됩니다. 문제는 프로파일링에 가파른 진입로가 있다는 것입니다. 흔적은 색깔이 있는 직사각형의 빽빽한 벽입니다. 이벤트에는 위협적인 이름이 있습니다. 대부분의 튜토리얼에서는 사용자가 이미 해당 튜토리얼을 읽을 수 있다고 가정합니다. 따라서 프로파일링을 해야 한다는 것을 알고 있더라도 추적을 여는 것은 나중(또는 다른 사람)을 위해 남겨 두는 것이 가장 좋은 자질구레한 일처럼 느껴질 수 있습니다. 이 게시물과 그것이 시작하는 시리즈는 진입로를 낮추려는 우리의 시도입니다. 이것은 프로파일러 추적을 읽는 기술을 천천히 구축하고 이를 사용하여 최적화를 추진하는 시리즈인 PyTorch에서의 프로파일링의 시작 게시물입니다. 그만큼계획: