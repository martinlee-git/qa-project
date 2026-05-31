# Chatgphish 취약점으로 인해 Chatgpt가 변경됨
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/05/chatgphish-vulnerability-turns-chatgpt.html
- Published At: unknown
- Collected At: 2026-05-31T13:43:59.514Z
- Notion Page: https://www.notion.so/The-Hacker-News-Chatgphish-Chatgpt-36ffc93aec5781a79cbeca86783bb155
- Original Title: Chatgphish Vulnerability Turns Chatgpt
## Summary
ChatGPhish는 ChatGPT Markdown 렌더링을 활용하여 요약된 웹 페이지에서 피싱 콘텐츠를 전달하여 AI 공격 표면을 늘립니다. 사이버 보안 연구원들이 마크다운 링크 및 이미지에 대한 인공 지능(AI) 비서의 암묵적 신뢰를 활용하여 즉각적인 주입을 유발하고 피싱 공격의 문을 여는 OpenAI ChatGPT의 취약점에 대한 세부 정보를 공개했습니다. 이 기술은 Permiso Security에 의해 ChatGphish라는 코드명으로 지정되었습니다. "chatgpt.com 응답 렌더러는 어시스턴트가 방금 요약한 제3자 페이지에서 시작된 마크다운 링크와 마크다운 이미지 URL을 신뢰합니다. 해당 이미지를 자동으로 가져오고 해당 링크를 내부에서 클릭 가능한 실시간 요소로 표시합니다…

## Original Description

ChatGPhish exploits ChatGPT Markdown rendering to deliver phishing content from summarized web pages, increasing AI attack surfaces.
## Key Points
- ChatGPhish는 ChatGPT Markdown 렌더링을 활용하여 요약된 웹 페이지에서 피싱 콘텐츠를 전달하여 AI 공격 표면을 늘립니다.
- 사이버 보안 연구원들이 마크다운 링크 및 이미지에 대한 인공 지능(AI) 비서의 암묵적 신뢰를 활용하여 즉각적인 주입을 유발하고 피싱 공격의 문을 여는 OpenAI ChatGPT의 취약점에 대한 세부 정보를 공개했습니다.
- 이 기술은 Permiso Security에 의해 ChatGphish라는 코드명으로 지정되었습니다.
## Excerpt
사이버 보안 연구원들이 마크다운 링크 및 이미지에 대한 인공 지능(AI) 비서의 암묵적 신뢰를 활용하여 즉각적인 주입을 유발하고 피싱 공격의 문을 여는 OpenAI ChatGPT의 취약점에 대한 세부 정보를 공개했습니다. 이 기술은 Permiso Security에 의해 ChatGphish라는 코드명으로 지정되었습니다. 보안 연구원인 Andi Ahmeti는 The Hacker News와 공유한 보고서에서 "chatgpt.com 응답 렌더러는 어시스턴트가 방금 요약한 제3자 페이지에서 시작된 마크다운 링크와 마크다운 이미지 URL을 신뢰합니다. 이러한 이미지를 자동으로 가져오고 해당 링크를 신뢰할 수 있는 어시스턴트 UI 내에 클릭 가능한 라이브 요소로 표시합니다"라고 말했습니다. 가상의 공격 시나리오에서 악의적인 행위자는 피해자가 나중에 ChatGPT에 요약하도록 요청하는 웹 페이지에 작은 페이로드를 추가하여 답변이 렌더링될 때 페이지에 포함된 공격자가 호스팅하는 이미지를 자동으로 가져올 때 IP, 사용자 에이전트 및 추천자 세부 정보가 유출되도록 할 수 있습니다. 또한 악성 Markdown 링크가 보조 응답 내에서 실시간 클릭 가능한 요소로 렌더링되고, 가짜 시스템 스타일 보안 경고를 제공하고, 공격자의 S3 버킷에서 QR 코드를 제공하고, 피해자가 모바일 장치를 통해 스캔하도록 속여 데스크톱 URL 필터 및 기업 보안 제어를 효과적으로 우회할 수 있습니다.