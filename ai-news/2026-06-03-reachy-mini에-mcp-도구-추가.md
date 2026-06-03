# Reachy Mini에 MCP 도구 추가
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/adding-mcp-tools-to-reachy-mini
- Published At: Wed, 03 Jun 2026 00:00:00 GMT
- Collected At: 2026-06-03T21:36:54.619Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-Reachy-Mini-MCP-374fc93aec578189afe0d2611d099c2f
- Original Title: Adding MCP Tools to Reachy Mini
## Summary
우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다. 내장 도구 프로필이 도구를 제어하는 ​​방법 로컬 도구의 한계 Spaces에서 도구 호출 설치, 나열, 제거 매니페스트가 있는 위치 도구 이름 지정 프로필 예 프롬프트가 중요한 이유 현재 작동하는 것과 작동하지 않는 것 도구 게시에 대한 팁 Space 결론 Reachy Mini 대화 앱은 이제 MCP를 통해 호출되는 공개 Hugging Face Spaces에서 호스팅되는 도구를 사용할 수 있습니다. 앱을 편집하는 대신 허브에서 스페이스를 추가하여 날씨 확인이나 웹 검색과 같은 새로운 기능을 로봇에 부여할 수 있습니다. 이 도구는 Space 자체에서 계속 실행되므로 코드가 다운로드되지 않습니다.

## Original Description

We’re on a journey to advance and democratize artificial intelligence through open source and open science.
## Key Points
- 우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다.
- 내장 도구 프로필이 도구를 제어하는 ​​방법 로컬 도구의 한계 Spaces에서 도구 호출 설치, 나열, 제거 매니페스트가 있는 위치 도구 이름 지정 프로필 예 프롬프트가 중요한 이유 현재 작동하는 것과 작동하지 않는 것 도구 게시에 대한 팁 Space 결론 Reachy Mini 대화 앱은 이제 MCP를 통해 호출되는 공개 Hugging Face Spaces에서 호스팅되는 도구를 사용할 수 있습니다.
- 앱을 편집하는 대신 허브에서 스페이스를 추가하여 날씨 확인이나 웹 검색과 같은 새로운 기능을 로봇에 부여할 수 있습니다.
## Excerpt
내장 도구 프로필이 도구를 제어하는 ​​방법 로컬 도구의 한계 Spaces에서 도구 호출 설치, 나열, 제거 매니페스트가 있는 위치 도구 이름 지정 프로필 예 프롬프트가 중요한 이유 현재 작동하는 것과 작동하지 않는 것 도구 게시에 대한 팁 Space 결론 Reachy Mini 대화 앱은 이제 MCP를 통해 호출되는 공개 Hugging Face Spaces에서 호스팅되는 도구를 사용할 수 있습니다. 앱을 편집하는 대신 허브에서 스페이스를 추가하여 날씨 확인이나 웹 검색과 같은 새로운 기능을 로봇에 부여할 수 있습니다. 이 도구는 Space 자체에서 계속 실행되므로 컴퓨터에 코드가 다운로드되지 않습니다. 그리고 다른 사람들이 사용할 수 있도록 자신만의 도구를 게시할 수도 있습니다. 아래에서는 도구가 무엇인지, 프로필이 로봇이 사용할 수 있는 것을 제어하는 ​​방법, 원격 경로의 현재 제한을 살펴봅니다. 로봇과 대화할 때 돌려받는 것은 음성뿐 아니라 대화에 반응하는 시스템입니다. 로봇은 해당되는 경우 비언어적으로 움직이고 응답할 수 있습니다. 여기서 우리가 집중하고 싶은 부분은 이를 가능하게 하는 도구입니다. 도구는 대화 중에 모델이 할 수 있는 작업입니다. 즉, 감정 표현, 머리 이동, 카메라를 통해 보기 등이 있습니다. 각 도구에는 이름과 간단한 설명이 있습니다. 모델은 이를 읽고, 언제 유용한지 결정하고, 호출한 다음, 반환되는 항목을 사용합니다. 오늘날 모든 도구는 로컬이며 앱 내부에 제공되며 대부분은 로봇 본체에 관한 것입니다. 코드의 도구는 여기에서 중요한 두 개의 파일이 있는 폴더인 profile 에서 활성화될 때까지 사용할 수 없습니다.Instructions.txt(프롬프트) 및 tools.txt(켜져 있는 도구)