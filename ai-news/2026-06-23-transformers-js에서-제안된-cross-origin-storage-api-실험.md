# Transformers.js에서 제안된 Cross-Origin Storage API 실험
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/cross-origin-storage
- Published At: Tue, 23 Jun 2026 00:00:00 GMT
- Collected At: 2026-06-23T19:10:36.429Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-Transformers-js-Cross-Origin-Storage-API-388fc93aec5781f1aaa2d2fcdc0f927b
- Original Title: Experimenting with the proposed Cross-Origin Storage API in Transformers.js
## Summary
우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다. 캐시 챌린지 모델 리소스 Wasm 런타임 리소스 캐시 격리 무엇을 읽을 수 있는 Cross-Origin Storage API 제어 입력 유틸리티를 희생하지 않는 무결성 디자인 프라이버시 Transformers.js 예제의 의미 오늘 시도해 보세요. 행동 유도(Google Chrome 팀의 개발자 관계 엔지니어 Thomas Steiner가 작성한 게스트 게시물입니다.) Transformers.js는 웹 개발자에게 작업별 파이프라인을 통해 웹 앱에서 변환기의 강력한 기능을 사용할 수 있는 간단한 방법을 제공합니다. 브라우저에서 추론을 실행하기 위해 개발자는 파이프라인() 인스턴스를 생성하고…

## Original Description

We’re on a journey to advance and democratize artificial intelligence through open source and open science.
## Key Points
- 우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다.
- 캐시 챌린지 모델 리소스 Wasm 런타임 리소스 캐시 격리 무엇을 읽을 수 있는 Cross-Origin Storage API 제어 입력 유틸리티를 희생하지 않는 무결성 디자인 프라이버시 Transformers.js 예제의 의미 오늘 시도해 보세요. 행동 유도(Google Chrome 팀의 개발자 관계 엔지니어 Thomas Steiner가 작성한 게스트 게시물입니다.) Transformers.js는 웹 개발자에게 작업별 파이프라인을 통해 웹 앱에서 변환기의 강력한 기능을 사용할 수 있는 간단한 방법을 제공합니다.
- 브라우저에서 추론을 실행하기 위해 개발자는 파이프라인() 인스턴스를 생성하고 파이프라인을 사용할 작업을 지정합니다.
## Excerpt
캐시 챌린지 모델 리소스 Wasm 런타임 리소스 캐시 격리 무엇을 읽을 수 있는 Cross-Origin Storage API 제어 입력 유틸리티를 희생하지 않는 무결성 디자인 프라이버시 Transformers.js 예제의 의미 오늘 시도해 보세요. 행동 유도(Google Chrome 팀의 개발자 관계 엔지니어 Thomas Steiner가 작성한 게스트 게시물입니다.) Transformers.js는 웹 개발자에게 작업별 파이프라인을 통해 웹 앱에서 변환기의 강력한 기능을 사용할 수 있는 간단한 방법을 제공합니다. 브라우저에서 추론을 실행하기 위해 개발자는 파이프라인() 인스턴스를 생성하고 파이프라인을 사용할 작업을 지정합니다. 구체적인 예로 다음 코드 조각은 자동 음성 인식(ASR) 파이프라인을 설정하는 방법을 보여줍니다. 소스 코드에서 제가 Xenova/whisper-tiny.en을 모델로 지정했다는 것을 알 수 있을 것입니다. 이는 일반적인 영어 자동 음성 인식 작업에 매우 적합한 선택입니다. 실제로 연결된 발췌문에 따르면 Transformers.js 기본 모델 해상도에 따른 기본 모델이기도 합니다. 브라우저에서 이 예제를 실행하면 Transformers.js가 자동으로 관련 모델 리소스 및 Wasm 파일을 다운로드하고 캐싱합니다. 다음 스크린샷은 앱 방문 후 Chrome DevTools 캐시 저장소 섹션을 보여줍니다. 페이지를 다시 로드하면 리소스가 Cache API에서 제공되고 모델은 거의 즉시 결과를 반환합니다. 그러나 Xenova/whisper-tiny.en은 인기 있는 모델입니다.이전에는 Transformers.js의 ASR 기본 모델이더라도 방문하는 하나 이상의 앱이 이를 사용할 것이라고 상상할 수 있습니다. 이 상황을 시뮬레이션하기 위해 이전과 동일한 예시 앱이 있지만 다른 출처에서 제공됩니다. 이 다른 출처 앱을 방문하면 오히려…