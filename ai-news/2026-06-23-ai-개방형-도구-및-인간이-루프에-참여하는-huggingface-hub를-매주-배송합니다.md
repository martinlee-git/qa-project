# AI, 개방형 도구 및 인간이 루프에 참여하는 Huggingface_hub를 매주 배송합니다.
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/huggingface-hub-release-ci
- Published At: Tue, 23 Jun 2026 00:00:00 GMT
- Collected At: 2026-06-23T08:03:36.197Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-AI-Huggingface_hub-388fc93aec57810eb6b6eea38428e0cf
- Original Title: Shipping huggingface_hub every week with AI, open tools, and a human in the loop
## Summary
우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다. 우리가 시작한 곳 두 가지 작업 설계 원칙: 누구나 재사용할 수 있는 개방형 부품 파이프라인 둘러보기 신뢰하되 검증: 인간 참여형 코어 문제를 구성하지 않도록 모델 접지 인간 체크포인트 개방적이고 안전한 배관 그렇다면 비용은 얼마나 듭니까? 실제로 변경된 사항 내 것으로 만들기 다음 단계 Huggingface_hub는 Hugging Face 생태계 기반의 Python 클라이언트입니다. 변환기, 데이터 세트, 디퓨저, 문장 변환기 및 기타 수십 개의 라이브러리가 허브와 통신하는 데 의존합니다. 매주 새 릴리스를 출시하지 않는 것은 수정하는 한 주입니다…

## Original Description

We’re on a journey to advance and democratize artificial intelligence through open source and open science.
## Key Points
- 우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다.
- 우리가 시작한 곳 두 가지 작업 설계 원칙: 누구나 재사용할 수 있는 개방형 부품 파이프라인 둘러보기 신뢰하되 검증: 인간 참여형 코어 문제를 구성하지 않도록 모델 접지 인간 체크포인트 개방적이고 안전한 배관 그렇다면 비용은 얼마나 듭니까?
- 실제로 변경된 사항 내 것으로 만들기 다음 단계 Huggingface_hub는 Hugging Face 생태계 기반의 Python 클라이언트입니다.
## Excerpt
우리가 시작한 곳 두 가지 작업 설계 원칙: 누구나 재사용할 수 있는 개방형 부품 파이프라인 둘러보기 신뢰하되 검증: 인간 참여형 코어 문제를 구성하지 않도록 모델 접지 인간 체크포인트 개방적이고 안전한 배관 그렇다면 비용은 얼마나 듭니까? 실제로 변경된 사항 내 것으로 만들기 다음 단계 Huggingface_hub는 Hugging Face 생태계 기반의 Python 클라이언트입니다. 변환기, 데이터 세트, 디퓨저, 문장 변환기 및 기타 수십 개의 라이브러리가 허브와 통신하는 데 의존합니다. 매주 새로운 릴리스를 출시하지 않는 한 주 동안은 수정 사항과 기능이 메인에 붙어 있습니다. 오랫동안 우리는 4~6주에 한 번씩 출시를 했습니다. 이제 우리는 단일 GitHub Actions 워크플로에서 매주 릴리스합니다. 우리는 오픈 소스 도구와 오픈 가중치 모델을 사용하여 이를 구축했으며 판단이 중요한 한 곳에서 인간이 계속해서 정보를 얻을 수 있도록 했습니다. 이 게시물에는 공급업체 계약, 폐쇄형 모델 또는 직접 실행할 수 없는 인프라가 필요하지 않습니다. 우리는 다른 유지관리자가 선택하고 적응할 수 있는 워크플로를 원했기 때문에 이것이 처음부터 설계 목표였습니다. 이 게시물이 끝나면 자신만의 것을 만드는 데 필요한 모든 것을 갖추게 될 것입니다. 이전 프로세스는 부분적으로 자동화되었으며 대부분 수동이었습니다. 새 버전에 대한 좋은 노트를 작성하는 것은 다양한 주제에 대한 수십 개의 PR을 모아서 무거운 부분이었습니다. 기술적으로 어려운 것은 없지만 몇 시간 동안 집중하면 됩니다. 상단에 공지 사항을 추가하면 마이너 릴리스는 쉽게 며칠에 걸쳐 반나절 작업이 이루어졌습니다.