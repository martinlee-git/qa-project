# Github에서 Actionscheckout을 차단하도록 업데이트
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/github-updates-actionscheckout-to-block.html
- Published At: unknown
- Collected At: 2026-06-23T22:11:37.984Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Github-Actionscheckout-388fc93aec578165aa9dd65bebaaa918
- Original Title: Github Updates Actionscheckout To Block
## Summary
GitHub의 작업/체크아웃 v7은 이제 권한 있는 워크플로에서 위험한 포크 PR 체크아웃을 차단하여 일반적인 pwn 요청 공격을 줄입니다. GitHub는 워크플로의 전체 권한으로 악성 코드를 실행하기 위해 "pull_request_target 워크플로" 트리거의 위험한 사용을 악용하는 pwn 요청 공격을 차단하기 위해 " actions/checkout"을 업데이트하여 소프트웨어 공급망 보안을 강화하기 위해 노력하고 있습니다. 2026년 6월 18일부터 워크플로 실행기로 저장소를 체크아웃하기 위한 공식 GitHub 작업인 "actions/checkout"의 최신 버전은 기본적으로 일반적인 pwn 요청 패턴을 거부합니다. 이 변경 사항은 2026년 7월 16일에 현재 지원되는 모든 주요 버전으로 백포트될 예정입니다. "작업/체크아웃…

## Original Description

GitHub’s actions/checkout v7 now blocks risky fork PR checkouts in privileged workflows to reduce common pwn request attacks.
## Key Points
- GitHub의 작업/체크아웃 v7은 이제 권한 있는 워크플로에서 위험한 포크 PR 체크아웃을 차단하여 일반적인 pwn 요청 공격을 줄입니다.
- GitHub는 워크플로의 전체 권한으로 악성 코드를 실행하기 위해 "pull_request_target 워크플로" 트리거의 위험한 사용을 악용하는 pwn 요청 공격을 차단하기 위해 " actions/checkout"을 업데이트하여 소프트웨어 공급망 보안을 강화하기 위해 노력하고 있습니다.
- 2026년 6월 18일부터 워크플로 실행기로 저장소를 체크아웃하기 위한 공식 GitHub 작업인 "actions/checkout"의 최신 버전은 기본적으로 일반적인 pwn 요청 패턴을 거부합니다.
## Excerpt
GitHub는 워크플로의 전체 권한으로 악성 코드를 실행하기 위해 "pull_request_target 워크플로" 트리거의 위험한 사용을 악용하는 pwn 요청 공격을 차단하기 위해 " actions/checkout"을 업데이트하여 소프트웨어 공급망 보안을 강화하기 위해 노력하고 있습니다. 2026년 6월 18일부터 워크플로 실행기로 저장소를 체크아웃하기 위한 공식 GitHub 작업인 "actions/checkout"의 최신 버전은 기본적으로 일반적인 pwn 요청 패턴을 거부합니다. 이 변경 사항은 2026년 7월 16일에 현재 지원되는 모든 주요 버전으로 백포트될 예정입니다. "Actions/checkout v7은 pull_request_target 및 Workflow_run 워크플로에서 포크 풀 요청 코드 가져오기를 거부합니다(후자는 Workflow_run.event가 pull_request* 이벤트인 경우에만 해당)"라고 덧붙였습니다. 거부는 풀 요청이 포크에서 발생하고 다음 기준 중 하나가 충족될 때 발생합니다. 단, 워크플로 작성자가 "actions/checkout"에서 "allow-unsafe-pr-checkout" 플래그를 "true"로 설정하여 이를 명시적으로 옵트아웃하지 않는 한, 변경 사항은 Actions 생태계에서 가장 일반적인 형태의 pwn 요청을 방지하는 것을 목표로 합니다. 결과적으로, 안전하지 않은 입력이 있는 포크의 "pull_request_target 이벤트"에 대해 "작업/체크아웃"이 실패합니다.