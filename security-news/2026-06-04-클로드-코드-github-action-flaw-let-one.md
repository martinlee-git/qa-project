# 클로드 코드 Github Action Flaw Let One
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/claude-code-github-action-flaw-let-one.html
- Published At: unknown
- Collected At: 2026-06-04T15:50:54.781Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Github-Action-Flaw-Let-One-375fc93aec57818595c4f25b0980ab69
- Original Title: Claude Code Github Action Flaw Let One
## Summary
Anthropic의 Claude Code GitHub Action의 결함으로 인해 봇 행위자의 악의적인 GitHub 문제가 워크플로를 트리거하고 저장소에 대한 쓰기 액세스 권한을 얻을 수 있었습니다. 보안 연구원은 Anthropic의 Claude Code GitHub Action에서 공격자가 단 하나의 GitHub 문제만 열어도 이를 실행하는 취약한 공개 저장소를 탈취할 수 있는 결함을 발견했습니다. Anthropic의 자체 작업 저장소가 동일한 작업 흐름을 사용했기 때문에 실제 공격으로 인해 악성 코드가 작업 자체와 이를 끌어오는 프로젝트 다운스트림에 푸시될 수 있었습니다. GMO Flatt Security의 RyotaK는 1월에 Anthropic에 핵심 우회를 보고했고 Anthropic은 이를 4일 이내에 수정했으며 봄까지 더욱 강화되었습니다. 티…

## Original Description

A flaw in Anthropic’s Claude Code GitHub Action allowed a malicious GitHub issue from a bot actor to trigger workflows and gain write access to repos.
## Key Points
- Anthropic의 Claude Code GitHub Action의 결함으로 인해 봇 행위자의 악의적인 GitHub 문제가 워크플로를 트리거하고 저장소에 대한 쓰기 액세스 권한을 얻을 수 있었습니다.
- 보안 연구원은 Anthropic의 Claude Code GitHub Action에서 공격자가 단 하나의 GitHub 문제만 열어도 이를 실행하는 취약한 공개 저장소를 탈취할 수 있는 결함을 발견했습니다.
- Anthropic의 자체 작업 저장소가 동일한 작업 흐름을 사용했기 때문에 실제 공격으로 인해 악성 코드가 작업 자체와 이를 끌어오는 프로젝트 다운스트림에 푸시될 수 있었습니다.
## Excerpt
보안 연구원은 Anthropic의 Claude Code GitHub Action에서 공격자가 단 하나의 GitHub 문제만 열어도 이를 실행하는 취약한 공개 저장소를 탈취할 수 있는 결함을 발견했습니다. Anthropic의 자체 작업 저장소가 동일한 작업 흐름을 사용했기 때문에 실제 공격으로 인해 악성 코드가 작업 자체와 이를 끌어오는 프로젝트 다운스트림에 푸시될 수 있었습니다. GMO Flatt Security의 RyotaK는 1월에 Anthropic에 핵심 우회를 보고했고 Anthropic은 이를 4일 이내에 수정했으며 봄까지 더욱 강화되었습니다. 수정 사항은 clude-code-action v1.0.94에 있습니다. Anthropic은 CVSS v4.0에서 문제를 7.8로 평가하고 버그 현상금을 지불했습니다. Claude Code GitHub Actions는 Claude를 CI/CD 파이프라인에 배치하여 문제 분류, 레이블 지정, 풀 요청 검토 또는 슬래시 명령 실행을 수행합니다. 기본적으로 워크플로는 저장소의 코드, 이슈, 끌어오기 요청, 토론 및 워크플로 파일에 대한 읽기 및 쓰기 액세스 권한을 갖습니다. 이러한 권한은 광범위하기 때문에 작업을 실행할 수 있는 사람이 까다로워야 합니다. 즉, 쓰기 액세스 권한이 있는 사용자만 해당 작업을 실행할 수 있습니다. 방아쇠 점검에 구멍이 생겼습니다. GitHub 앱은 관리자가 설치하는 신뢰할 수 있는 앱이라는 가정 하에 이름이 [bot]으로 끝나는 모든 행위자를 통해 전달되었습니다. 문제는 누구나 GitHub 앱을 등록하고, 자신이 소유한 리포지토리에 설치하고, 해당 토큰을 사용하여 공개 리포지토리에서 이슈를 열거나 풀 요청을 할 수 있다는 것입니다. 이 작업은 "봇"을 확인하고 공격자의 콘텐츠를 통과시킵니다. 태그 모드에는 배우가 실제 인간인지 확인하기 위한 추가 검사가 있었습니다. 대리인모드가 실행되지 않아서 열려 있었습니다. 여기에서 공격자는 AI가 읽는 콘텐츠 내에 지침을 심어 모델이 실제 작업 대신 이를 따르도록 하는 비법인 간접 프롬프트 주입에 의존합니다. RyotaK는 본문이 오류 메시지처럼 보이는 문제를 작성한 다음 무도회를 다듬었습니다…