# 원클릭 Github Dev 공격 허용
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/one-click-github-dev-attack-lets.html
- Published At: unknown
- Collected At: 2026-06-03T13:32:55.478Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Github-Dev-374fc93aec5781429a3bda143454c3fd
- Original Title: One Click Github Dev Attack Lets
## Summary
VS Code 결함은 GitHub.dev에 대한 원클릭 공격을 통해 GitHub OAuth 토큰을 노출시켜 개인 저장소 액세스 및 토큰 도용을 가능하게 합니다. 사이버 보안 연구원들이 사용자의 GitHub 토큰을 훔칠 수 있는 Microsoft Visual Studio Code(VS Code)를 통한 원클릭 공격을 공개했습니다. 보안 연구원 Ammar Askar는 "링크를 클릭하는 것만으로도 공격자가 개인 저장소를 포함하여 저장소를 읽고 쓸 수 있는 GitHub 토큰을 훔칠 수 있습니다"라고 말했습니다. GitHub는 VS Code 환경을 시작하여 웹 브라우저의 샌드박스에서 경량 웹 기반 소스 코드 편집기로 실행되는 GitHub.dev라는 기능을 지원합니다. 이를 통해 사용자는 풀 요청을 보내고 커밋을 할 수 있습니다. "이 기능은…

## Original Description

VS Code flaw exposes GitHub OAuth tokens via one-click attack on GitHub.dev, enabling private repo access and token theft.
## Key Points
- VS Code 결함은 GitHub.dev에 대한 원클릭 공격을 통해 GitHub OAuth 토큰을 노출시켜 개인 저장소 액세스 및 토큰 도용을 가능하게 합니다.
- 사이버 보안 연구원들이 사용자의 GitHub 토큰을 훔칠 수 있는 Microsoft Visual Studio Code(VS Code)를 통한 원클릭 공격을 공개했습니다.
- 보안 연구원 Ammar Askar는 "링크를 클릭하는 것만으로도 공격자가 개인 저장소를 포함하여 저장소를 읽고 쓸 수 있는 GitHub 토큰을 훔칠 수 있습니다"라고 말했습니다.
## Excerpt
사이버 보안 연구원들이 사용자의 GitHub 토큰을 훔칠 수 있는 Microsoft Visual Studio Code(VS Code)를 통한 원클릭 공격을 공개했습니다. 보안 연구원 Ammar Askar는 "링크를 클릭하는 것만으로도 공격자가 개인 저장소를 포함하여 저장소를 읽고 쓸 수 있는 GitHub 토큰을 훔칠 수 있습니다"라고 말했습니다. GitHub는 VS Code 환경을 시작하여 웹 브라우저의 샌드박스에서 경량 웹 기반 소스 코드 편집기로 실행되는 GitHub.dev라는 기능을 지원합니다. 이를 통해 사용자는 풀 요청을 보내고 커밋을 할 수 있습니다. Askar는 "이 기능은 github.com이 사용자를 대신하여 GitHub와 상호 작용할 수 있도록 OAuth 토큰을 github.dev에 게시함으로써 달성됩니다"라고 말했습니다. "토큰은 사용자가 상호작용한 특정 저장소로 범위가 지정되지 않습니다. 즉, 사용자가 액세스할 수 있는 다른 모든 저장소에 대한 전체 액세스 권한을 갖습니다." 간단히 말해서, 이 취약점을 통해 공격자는 기본 VS Code 창과 webview 사이의 메시지 전달 메커니즘을 이용하여 GitHub OAuth 토큰이 GitHub.dev에 전달될 때 이를 훔치는 악성 VS Code 확장을 설치할 수 있습니다. Webview는 Markdown 미리 보기를 렌더링하거나 Jupyter 노트북을 편집하는 데 사용됩니다.