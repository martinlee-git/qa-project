# North Mini Code 소개: 개발자를 위한 Cohere의 첫 번째 모델
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/CohereLabs/introducing-north-mini-code
- Published At: Tue, 09 Jun 2026 15:56:23 GMT
- Collected At: 2026-06-11T20:48:47.438Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-North-Mini-Code-Cohere-37afc93aec5781558ebdc8ab22108578
- Original Title: Introducing North Mini Code: Cohere’s First Model For Developers
## Summary
Hugging Face Architecture에 대한 Cohere Labs의 블로그 게시물 하네스 전반에 걸친 코딩 우수성 견고성에 대한 포스트 트레이닝 에이전트 코딩을 위한 비동기 RL 내부 인간 평가 벤치마크 시작하기 확장 작성자 목록 벤치마킹 방법론 인용 참조 각주 아래 나열된 모든 공동 저자는 오늘 강력한 에이전트 코딩 기능을 갖춘 30B 활성 매개변수를 갖춘 30B 매개변수 전문가 혼합 모델인 North Mini Code를 출시합니다. Apache 2.0 라이센스에 따라 Hugging Face에 대해 설명합니다. North Mini Code는 Cohere의 새로운 모델 제품군 중 첫 번째 모델이며 에이전트 소프트웨어 엔지니어링 작업을 위해 특별히 설계되고 훈련되었습니다. 그림 1: North Mini Code의 성능…

## Original Description

A Blog post by Cohere Labs on Hugging Face
## Key Points
- Hugging Face Architecture에 대한 Cohere Labs의 블로그 게시물 하네스 전반에 걸친 코딩 우수성 견고성에 대한 포스트 트레이닝 에이전트 코딩을 위한 비동기 RL 내부 인간 평가 벤치마크 시작하기 확장 작성자 목록 벤치마킹 방법론 인용 참조 각주 아래 나열된 모든 공동 저자는 오늘 강력한 에이전트 코딩 기능을 갖춘 30B 활성 매개변수를 갖춘 30B 매개변수 전문가 혼합 모델인 North Mini Code를 출시합니다. Apache 2.0 라이센스에 따라 Hugging Face에 대해 설명합니다.
- North Mini Code는 Cohere의 새로운 모델 제품군 중 첫 번째 모델이며 에이전트 소프트웨어 엔지니어링 작업을 위해 특별히 설계되고 훈련되었습니다.
- 그림 1: 유사한 규모의 주요 오픈 소스 모델과 비교한 에이전트 코딩 작업 및 복잡한 코드 생성 벤치마크에서 North Mini Code의 성능.
## Excerpt
코딩 우수성을 위한 아키텍처 사후 교육 하네스 전반의 견고성 에이전트 코딩을 위한 비동기 RL 내부 인간 평가 벤치마크 시작하기 확장된 저자 목록 벤치마킹 방법론 인용 참조 각주 아래 나열된 모든 공동 저자 오늘 우리는 강력한 에이전트 코딩 기능을 갖춘 30B 매개변수 전문가 혼합 모델인 North Mini Code를 출시합니다. 이는 Apache 2.0 라이선스에 따라 Hugging Face에서 사용할 수 있습니다. North Mini Code는 Cohere의 새로운 모델 제품군 중 첫 번째 모델이며 에이전트 소프트웨어 엔지니어링 작업을 위해 특별히 설계되고 훈련되었습니다. 그림 1: 유사한 규모의 주요 오픈 소스 모델과 비교한 에이전트 코딩 작업 및 복잡한 코드 생성 벤치마크에서 North Mini Code의 성능. 벤치마킹 방법론에 대한 자세한 내용은 여기를 참조하세요. North Mini Code는 복잡한 소프트웨어 엔지니어링 워크플로, 터미널 기반 에이전트 작업 및 고품질 코드 생성에 최적화되어 있습니다. 인공 분석의 코딩 지수에서 North Mini Code는 33.4점을 달성하여 Qwen3.5(35B-A3B), Gemma 4(26B-A4B), Devstral Small 2(24B Dense) 및 Nemotron 3 Super(120B-A12B), Mistral Small 4(119B-A6B) 및 Devstral 2와 같은 훨씬 더 큰 모델보다 성능이 뛰어납니다. (123B). 1 해당 크기 등급에서 가장 강력한 오픈 소스 코딩 모델 중 하나입니다.