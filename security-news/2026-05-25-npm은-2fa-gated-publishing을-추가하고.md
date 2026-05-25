# Npm은 2fa Gated Publishing을 추가하고
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/05/npm-adds-2fa-gated-publishing-and.html
- Published At: unknown
- Collected At: 2026-05-25T15:39:25.100Z
- Notion Page: https://www.notion.so/The-Hacker-News-Npm-2fa-Gated-Publishing-36bfc93aec5781429925e363dcefeca1
- Original Title: Npm Adds 2fa Gated Publishing And
## Summary
GitHub는 소프트웨어 공급망 공격 위험을 줄이기 위해 필수 2FA 승인과 함께 npm 단계적 게시를 추가했습니다. GitHub는 소프트웨어 공급망의 보안을 개선하기 위해 npm에 대한 새로운 제어 기능을 출시하여 관리자가 패키지를 공개적으로 설치하기 전에 릴리스를 명시적으로 승인할 수 있는 기능을 제공합니다. 단계적 게시라고 하는 이 기능은 이제 npm에서 일반적으로 사용할 수 있습니다. 패키지가 npmjs[.]com에 푸시되기 전에 인간 유지 관리자가 2단계 인증(2FA) 챌린지를 통과하여 패키지를 승인하도록 요구합니다. "소비자에게 패키지 버전을 즉시 제공하는 직접 게시 대신 사전 빌드된 타르볼이 스테이지 대기열에 업로드됩니다…

## Original Description

GitHub added npm staged publishing with mandatory 2FA approval to reduce software supply chain attack risks.
## Key Points
- GitHub는 소프트웨어 공급망 공격 위험을 줄이기 위해 필수 2FA 승인과 함께 npm 단계적 게시를 추가했습니다.
- GitHub는 소프트웨어 공급망의 보안을 개선하기 위해 npm에 대한 새로운 제어 기능을 출시하여 관리자가 패키지를 공개적으로 설치하기 전에 릴리스를 명시적으로 승인할 수 있는 기능을 제공합니다.
- 단계적 게시라고 하는 이 기능은 이제 npm에서 일반적으로 사용할 수 있습니다.
## Excerpt
GitHub는 소프트웨어 공급망의 보안을 개선하기 위해 npm에 대한 새로운 제어 기능을 출시하여 관리자가 패키지를 공개적으로 설치하기 전에 릴리스를 명시적으로 승인할 수 있는 기능을 제공합니다. 단계적 게시라고 하는 이 기능은 이제 npm에서 일반적으로 사용할 수 있습니다. 패키지가 npmjs[.]com에 푸시되기 전에 인간 유지 관리자가 2단계 인증(2FA) 챌린지를 통과하여 패키지를 승인하도록 요구합니다. GitHub는 "소비자에게 패키지 버전을 즉시 제공하는 직접 게시 대신 미리 빌드된 타르볼이 설치 가능해지기 전에 관리자가 명시적으로 승인해야 하는 단계 대기열에 업로드됩니다."라고 말했습니다. 마이크로소프트 소유 자회사는 이번 변경으로 비대화형 CI/CD 워크플로우와 OIDC(OpenID Connect) 인증을 통한 신뢰할 수 있는 게시를 포함하여 모든 게시에 대해 "존재 증명"이 보장된다고 밝혔습니다. 단계적 게시를 사용하기 전에 패키지 관리자는 다음 기준을 충족해야 합니다.