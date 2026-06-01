# Reachy Mini는 완전히 로컬로 작동합니다.
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/local-reachy-mini-conversation
- Published At: Wed, 27 May 2026 00:00:00 GMT
- Collected At: 2026-06-01T11:58:57.210Z
- Notion Page: https://www.notion.so/Hugging-Face-Blog-Reachy-Mini-36dfc93aec5781f7b8f1e20529cefac2
- Original Title: Reachy Mini goes fully local
## Summary
우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다. 빠른 시작 로컬에서 LLM 제공 음성-음성 설정 Reachy Mini를 음성-음성으로 연결 심층 분석 자체 음성-음성 서버를 실행하는 이유는 무엇입니까? 우리가 주장하는 기본값: VAD, STT, TTS LLM 선택 노트북에서 엔진 실행, 로봇의 앱 요약 Reachy Mini를 만든 후 대화 앱을 설치하고 대화를 시작합니다. 지금까지는 오디오를 서버로 보내야 했습니다. 하지만 더 이상은 아닙니다. 오늘은 전체 스택을 로컬에서 실행하는 방법을 안내해 드리겠습니다. 이 스택은 계단식 VAD → STT → LLM → TTS 파이프인 음성 대 음성으로 구동됩니다.

## Original Description

We’re on a journey to advance and democratize artificial intelligence through open source and open science.
## Key Points
- 우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다.
- 빠른 시작 로컬에서 LLM 제공 음성-음성 설정 Reachy Mini를 음성-음성으로 연결 심층 분석 자체 음성-음성 서버를 실행하는 이유는 무엇입니까?
- 우리가 주장하는 기본값: VAD, STT, TTS LLM 선택 노트북에서 엔진 실행, 로봇의 앱 요약 Reachy Mini를 만든 후 대화 앱을 설치하고 대화를 시작합니다.
## Excerpt
빠른 시작 로컬에서 LLM 제공 음성-음성 설정 Reachy Mini를 음성-음성으로 연결 심층 분석 자체 음성-음성 서버를 실행하는 이유는 무엇입니까? 우리가 주장하는 기본값: VAD, STT, TTS LLM 선택 노트북에서 엔진 실행, 로봇의 앱 요약 Reachy Mini를 만든 후 대화 앱을 설치하고 대화를 시작합니다. 지금까지는 오디오를 서버로 보내야 했습니다. 하지만 더 이상은 아닙니다. 오늘은 전체 스택을 로컬에서 실행하는 방법을 안내해 드리겠습니다. 이 스택은 Realtime API 호환 /v1/realtime WebSocket을 노출하는 계단식 VAD → STT → LLM → TTS 파이프라인인 음성-음성 으로 구동됩니다. 백엔드를 실행한 후 UI에서 로봇이 백엔드를 가리키도록 하세요. 캐스케이드는 오늘날 오픈 소스 환경에서 가장 유연한 옵션이며 올바른 부분을 사용하면 가장 빠릅니다. 우리는 가장 마음에 드는 구성 요소를 추천해 주지만 캐스케이드의 핵심은 구성 요소를 교체할 수 있다는 것입니다. 매주 새로운 모델이 출시됩니다. 이 블로그에서는 완전히 로컬에서 Reachy Mini와 대화를 실행하는 과정을 안내합니다. 클라우드도 없고, API 키도 없고, 데이터가 컴퓨터에서 나가지 않습니다. 다음은 이를 실시간으로 보여주는 비디오입니다. LLM을 제공하기 위해 Hugging Face의 llama.cpp를 사용하겠습니다. 설치해야 하는 경우 가장 간단한 방법은 Brew install llama.cpp 또는 Winget install llama.cpp 입니다. 자세한 내용은 문서를 확인하세요. 먼저 다음을 실행합니다.