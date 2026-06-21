# DiffusionGemma: 4배 더 빠른 텍스트 생성
- Source: Google DeepMind
- Category: ai_news
- Original URL: https://deepmind.google/blog/diffusiongemma-4x-faster-text-generation/
- Published At: Wed, 10 Jun 2026 16:24:11 +0000
- Collected At: 2026-06-21T02:24:40.615Z
- Notion Page: https://app.notion.com/p/Google-DeepMind-DiffusionGemma-4-37bfc93aec5781679468f3a32fa23158
- Original Title: DiffusionGemma: 4x faster text generation
## Summary
최대 4배 더 빠른 속도를 제공하는 매우 빠른 텍스트 생성 모델인 DiffusionGemma에 대한 개요입니다. 최신 개방형 실험 모델은 전용 GPU에서 최대 4배 더 빠른 추론을 제공하고 속도가 중요한 대화형 로컬 워크플로를 탐색할 수 있는 기회를 열어줍니다. 오늘 우리는 텍스트 생성에 대한 매우 빠른 접근 방식인 텍스트 확산을 탐색하는 실험적인 개방형 모델인 DiffusionGemma를 소개합니다. Apache 2.0 라이선스에 따라 출시된 이 26B 전문가 혼합(MoE) 모델은 일반적인 자동 회귀 LLM(대형 언어 모델)의 토큰별 순차적 처리를 뛰어넘습니다. 대신, 전체 텍스트 블록을 동시에 생성하여 최대 4배 빠른 텍스트 전달 속도를 제공합니다.

## Original Description

An overview of DiffusionGemma, an exceptionally fast text generation model with up to 4x faster speeds.
## Key Points
- 최대 4배 더 빠른 속도를 제공하는 매우 빠른 텍스트 생성 모델인 DiffusionGemma에 대한 개요입니다.
- 최신 개방형 실험 모델은 전용 GPU에서 최대 4배 더 빠른 추론을 제공하고 속도가 중요한 대화형 로컬 워크플로를 탐색할 수 있는 기회를 열어줍니다.
- 오늘 우리는 텍스트 생성에 대한 매우 빠른 접근 방식인 텍스트 확산을 탐색하는 실험적인 개방형 모델인 DiffusionGemma를 소개합니다.
## Excerpt
최신 개방형 실험 모델은 전용 GPU에서 최대 4배 더 빠른 추론을 제공하고 속도가 중요한 대화형 로컬 워크플로를 탐색할 수 있는 기회를 열어줍니다. 오늘 우리는 텍스트 생성에 대한 매우 빠른 접근 방식인 텍스트 확산을 탐색하는 실험적인 개방형 모델인 DiffusionGemma를 소개합니다. Apache 2.0 라이선스에 따라 출시된 이 26B 전문가 혼합(MoE) 모델은 일반적인 자동 회귀 LLM(대형 언어 모델)의 토큰별 순차적 처리를 뛰어넘습니다. 대신 전체 텍스트 블록을 동시에 생성하여 GPU에서 텍스트 생성 속도가 최대 4배 더 빨라집니다. Gemma 4 제품군의 업계 최고의 매개변수당 지능과 최첨단 Gemini Diffusion 연구를 기반으로 구축된 DiffusionGemma는 생성 ​​속도를 최대화하도록 설계된 새로운 확산 헤드를 통합합니다. 자동 회귀 Gemma 4 모델은 고품질 생산 출력의 표준으로 남아 있지만 DiffusionGemma는 인라인 편집, 빠른 반복 및 비선형 텍스트 구조 생성과 같이 속도가 중요한 대화형 로컬 워크플로우를 탐색하는 연구원 및 개발자를 위해 설계되었습니다. 실시간 대화형 AI 애플리케이션을 구축하는 개발자는 로컬 추론의 지연 병목 현상으로 인해 어려움을 겪는 경우가 많습니다. DiffusionGemma는 몇 가지 주요 장단점을 통해 이러한 문제를 직접적으로 해결합니다. 미세 조정을 통해 특정 작업에 대한 DiffusionGemma의 성능을 향상시킬 수 있습니다. 아래 예에서 Unsloth는 작업 자동 회귀 모드인 Sudoku를 플레이하기 위해 DiffusionGemma를 미세 조정했습니다.각 토큰은 미래 토큰에 의존하기 때문에 어려움을 겪습니다. DiffusionGemma의 양방향 관심은 이를 훨씬 쉽게 만듭니다.