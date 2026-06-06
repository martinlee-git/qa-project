# Thousand Token Wood: 3B 모델로 다중 에이전트 경제 제공
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/build-small-hackathon/thousand-token-wood-sim
- Published At: Fri, 05 Jun 2026 22:18:46 GMT
- Collected At: 2026-06-06T05:18:51.896Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-Thousand-Token-Wood-3B-376fc93aec5781eb96d5d7592965b53b
- Original Title: Thousand Token Wood: shipping a multi-agent economy on a 3B model
## Summary
Hugging Face에 대한 Build Small Hackathon의 블로그 게시물 왜 디자인이 한계가 아니라 작은가 첫 번째 경제는 도착하자마자 죽었습니다 유효한 JSON, 약한 판단 그런 다음 이야기를 하기 시작했습니다. 먼저 시도해 보세요: Space 및 오픈 에이전트 추적. 저는 Build Small Hackathon을 위해 Thousand Token Wood를 만들었습니다. 이것은 작은 경제입니다. 각각 Qwen2.5-3B의 에이전트인 5마리의 삼림지대 생물이 5개의 상품을 자갈, 가십, 보물, 공황과 교환합니다. 나무를 찌르고 거품, 붕괴, 부의 격차가 저절로 커지는 것을 지켜보세요…

## Original Description

A Blog post by Build Small Hackathon on Hugging Face
## Key Points
- Hugging Face에 대한 Build Small Hackathon의 블로그 게시물 왜 디자인이 한계가 아니라 작은가 첫 번째 경제는 도착하자마자 죽었습니다 유효한 JSON, 약한 판단 그런 다음 이야기를 하기 시작했습니다.
- 먼저 시도해 보세요: Space 및 오픈 에이전트 추적.
- 저는 Build Small Hackathon을 위해 Thousand Token Wood를 만들었습니다.
## Excerpt
한계가 아니라 작은 디자인이 필요한 이유 첫 번째 경제는 도착하자마자 죽었습니다. 유효한 JSON, 약한 판단 그런 다음 실제로 일어난 일을 이야기하기 시작했습니다. 작은 모델로 구축하기 위한 요점 30억 매개변수 거래자 협의회가 할 수 있는 것과 할 수 없는 것에 대한 Build Small Hackathon 현장 보고서. 먼저 시도해 보세요: Space 및 오픈 에이전트 추적. 저는 Build Small Hackathon을 위해 Thousand Token Wood를 만들었습니다. 이것은 작은 경제입니다. 각각 Qwen2.5-3B의 에이전트인 5마리의 삼림지대 생물이 5개의 상품을 자갈, 가십, 보물, 공황과 교환합니다. 당신은 나무를 찌르고 거품, 붕괴, 넓어지는 부의 격차가 저절로 나타나는 것을 지켜봅니다. 이 모델은 Modal에서 vLLM과 함께 제공됩니다. Gradio 앱은 나무 위의 창입니다. 이 글은 작은 모형을 제작하는 사람들을 위해 작성된 엔지니어링 현장 보고서입니다. 짧은 버전: 3B 모델은 신뢰할 수 있는 형식 생성기이자 신뢰할 수 없는 추론기이며, 새로운 시스템에는 설계된 희소성이 필요하며, 최고의 데모는 기술적 제약이 이미 깊이 이해하고 있는 것과 만나는 곳에 있습니다. 살아있는 경제에는 실행당 여러 번 생각하는 많은 에이전트가 필요합니다. 이것이 바로 프런티어 모델이 잘못된 도구인 부분입니다. 매 틱마다 트레이더 협의회를 운영하기에는 너무 느리고 비용이 너무 많이 듭니다. 작은 모델은 실시간 다중 에이전트 시뮬레이션을 가능하게 만듭니다. 모든 생물은 턴당 단일 일괄 GPU 호출을 통해 결정합니다.