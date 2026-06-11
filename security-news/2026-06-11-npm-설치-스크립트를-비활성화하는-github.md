# Npm 설치 스크립트를 비활성화하는 Github
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/github-to-disable-npm-install-scripts.html
- Published At: unknown
- Collected At: 2026-06-11T09:41:47.773Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Npm-Github-37cfc93aec5781a5999cf47d76a5c646
- Original Title: Github To Disable Npm Install Scripts
## Summary
npm 12는 기본적으로 설치 스크립트를 비활성화하므로 종속성 기반 코드 실행 위험을 줄이기 위해 명시적인 승인이 필요합니다. GitHub는 npm 버전 12에 대한 "획기적인 변경 사항"을 발표했습니다. 이 중 하나는 소프트웨어 공급망 위협에 맞서기 위해 기본적으로 설치 스크립트를 비활성화합니다. 변경 사항의 목적은 npm 수명 주기 후크를 사용하여 악성 코드 실행을 트리거하기 위해 "npm install" 명령을 남용하는 공격 기술에 맞서는 것입니다. "Npm install"은 Node.js 프로젝트에 필요한 모든 종속성을 다운로드하고 설치하는 데 사용됩니다. 버전 12는 다음 달 출시될 예정입니다. 설치 시간 라이프사이클 스크립트를 "npm ecosys에서 가장 큰 단일 코드 실행 표면으로 설명…

## Original Description

npm 12 disables install scripts by default, requiring explicit approval to reduce dependency-based code execution risks.
## Key Points
- npm 12는 기본적으로 설치 스크립트를 비활성화하므로 종속성 기반 코드 실행 위험을 줄이기 위해 명시적인 승인이 필요합니다.
- GitHub는 npm 버전 12에 대한 "획기적인 변경 사항"을 발표했습니다. 이 중 하나는 소프트웨어 공급망 위협에 맞서기 위해 기본적으로 설치 스크립트를 비활성화합니다.
- 변경 사항의 목적은 npm 수명 주기 후크를 사용하여 악성 코드 실행을 트리거하기 위해 "npm install" 명령을 남용하는 공격 기술에 맞서는 것입니다.
## Excerpt
GitHub는 npm 버전 12에 대한 "획기적인 변경 사항"을 발표했습니다. 이 중 하나는 소프트웨어 공급망 위협에 맞서기 위해 기본적으로 설치 스크립트를 비활성화합니다. 변경 사항의 목적은 npm 수명 주기 후크를 사용하여 악성 코드 실행을 트리거하기 위해 "npm install" 명령을 남용하는 공격 기술에 맞서는 것입니다. "Npm install"은 Node.js 프로젝트에 필요한 모든 종속성을 다운로드하고 설치하는 데 사용됩니다. 버전 12는 다음 달 출시될 예정입니다. GitHub는 설치 시간 라이프사이클 스크립트를 "npm 생태계에서 가장 큰 단일 코드 실행 표면"으로 설명하면서 "npm install" 명령은 모든 전이적 종속성에서 스크립트를 실행하며 그 결과 종속성 트리의 어느 곳에서든 손상된 단일 패키지가 개발자 시스템 또는 CI 실행기에서 임의의 코드를 실행할 수 있다고 말했습니다. 이러한 동작을 차단함으로써 기본적으로 신뢰되는 것이 아니라 "npm install" 중에 코드 실행이 자동으로 시작되기 전에 명시적인 사용자 승인을 요구한다는 아이디어입니다. GitHub는 "스크립트 실행을 옵트인으로 설정하면 해당 경로가 닫히고 신뢰하는 패키지에 대해 하나의 명령만 유지됩니다."라고 말했습니다. "여기에는 기본 node-gyp 빌드가 포함됩니다(즉, npm이 암시적 node-gyp 재구축을 실행하기 때문에 바인딩.gyp이 있고 명시적 설치 스크립트가 없는 패키지는 여전히 차단됩니다."라고 Microsoft 소유 자회사는 기본 "allowScripts" 동작 변경에 대해 말했습니다. "git, 파일 및 링크 종속성에서 스크립트 준비는 동일한 방식으로 차단됩니다."