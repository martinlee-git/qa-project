# 새로운 Frost Attack으로 웹사이트 추적 가능
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/new-frost-attack-lets-websites-track.html
- Published At: unknown
- Collected At: 2026-06-09T12:11:51.323Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Frost-Attack-37afc93aec5781bdb695e3586eafc445
- Original Title: New Frost Attack Lets Websites Track
## Summary
FROST는 JavaScript 및 OPFS SSD 타이밍을 사용하여 88.95% F1에서 웹 사이트를 식별하여 브라우저 간 개인 정보 유출을 노출합니다. 악성 웹사이트는 JavaScript와 SSD 타이밍만을 사용하여 사용자가 방문하는 사이트와 여는 앱을 알아낼 수 있습니다. FROST라고 불리는 이 공격에는 네이티브 코드, 확장자, 권한 프롬프트가 필요하지 않습니다. 페이지를 열고 탭을 그대로 두면 백그라운드에서 경합이 일어나는지 지켜봅니다. Graz University of Technology의 연구원들은 이를 구축하고 DIMVA 2026에 발표될 새로운 논문 세트에서 이를 설명했습니다. 이는 모든 주요 데스크톱 브라우저에 있는 저장 기능을 남용하며 기본 타이밍 채널은 macOS와 Linux 모두에서 작동합니다. SSD…

## Original Description

FROST uses JavaScript and OPFS SSD timing to identify websites at 88.95% F1, exposing cross-browser privacy leaks.
## Key Points
- FROST는 JavaScript 및 OPFS SSD 타이밍을 사용하여 88.95% F1에서 웹 사이트를 식별하여 브라우저 간 개인 정보 유출을 노출합니다.
- 악성 웹사이트는 JavaScript와 SSD 타이밍만을 사용하여 사용자가 방문하는 사이트와 여는 앱을 알아낼 수 있습니다.
- FROST라고 불리는 이 공격에는 네이티브 코드, 확장자, 권한 프롬프트가 필요하지 않습니다.
## Excerpt
악성 웹사이트는 JavaScript와 SSD 타이밍만을 사용하여 사용자가 방문하는 사이트와 여는 앱을 알아낼 수 있습니다. FROST라고 불리는 이 공격에는 네이티브 코드, 확장자, 권한 프롬프트가 필요하지 않습니다. 페이지를 열고 탭을 그대로 두면 백그라운드에서 경합이 일어나는지 지켜봅니다. Graz University of Technology의 연구원들은 이를 구축하고 DIMVA 2026에 발표될 새로운 논문 세트에서 이를 설명했습니다. 이는 모든 주요 데스크톱 브라우저에 있는 저장 기능을 남용하며 기본 타이밍 채널은 macOS와 Linux 모두에서 작동합니다. SSD 타이밍 공격은 새로운 것이 아닙니다. 작년에 같은 그룹은 다른 사람이 드라이브를 사용할 때 읽기 속도가 어떻게 느려지는지 관찰하여 드라이브에서 사용자 행동을 읽는 Secret Spilling Drive를 발표했습니다. 문제는 Linux의 io_uring과 같은 저수준 인터페이스를 통해 머신에 네이티브 코드가 필요하다는 것이었습니다. FROST는 해당 요구 사항을 삭제합니다. 브라우저 샌드박스 내에서 실행되어 로컬 공격을 원격 공격으로 전환합니다. 더 이상 기계를 꺼내기 위해 기계 위에 있을 필요가 없습니다.