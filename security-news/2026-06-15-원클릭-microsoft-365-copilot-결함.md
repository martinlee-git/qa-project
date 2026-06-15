# 원클릭 Microsoft 365 Copilot 결함
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/one-click-microsoft-365-copilot-flaw.html
- Published At: unknown
- Collected At: 2026-06-15T15:49:44.750Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Microsoft-365-Copilot-380fc93aec5781c7b459f4b50c6dbe77
- Original Title: One Click Microsoft 365 Copilot Flaw
## Summary
Microsoft는 하나의 신뢰할 수 있는 링크를 통해 이메일, 달력 및 색인화된 파일을 노출할 수 있는 심각한 Copilot Enterprise Search 결함을 수정했습니다. 신뢰할 수 있는 Microsoft 링크를 한 번만 클릭하면 공격자가 Microsoft 365 Copilot Enterprise Search에서 이메일, 일정 세부 정보 및 색인화된 파일을 가져올 수 있습니다. Varonis Threat Labs의 연구원들은 SearchLeak이라고 하는 원클릭 유출 경로에 3개의 버그를 연결했습니다. 링크가 실제 microsoft.com 도메인을 가리키기 때문에 기존의 피싱 방지 및 URL 필터링 도구에서는 해당 도메인에 플래그를 지정할 가능성이 없습니다. 메시지도 없고, 비밀번호도 없고, 두 번째 클릭도 없습니다. Microsoft는 CVE-2026-42824를 할당하고 중요로 표시했습니다. CVSS 점수는 6.5점으로 더 낮았고 동의하지 않았습니다.

## Original Description

Microsoft fixed a critical Copilot Enterprise Search flaw that could expose emails, calendars, and indexed files through one trusted link.
## Key Points
- Microsoft는 하나의 신뢰할 수 있는 링크를 통해 이메일, 달력 및 색인화된 파일을 노출할 수 있는 심각한 Copilot Enterprise Search 결함을 수정했습니다.
- 신뢰할 수 있는 Microsoft 링크를 한 번만 클릭하면 공격자가 Microsoft 365 Copilot Enterprise Search에서 이메일, 일정 세부 정보 및 색인화된 파일을 가져올 수 있습니다.
- Varonis Threat Labs의 연구원들은 SearchLeak이라고 하는 원클릭 유출 경로에 3개의 버그를 연결했습니다.
## Excerpt
신뢰할 수 있는 Microsoft 링크를 한 번만 클릭하면 공격자가 Microsoft 365 Copilot Enterprise Search에서 이메일, 일정 세부 정보 및 색인화된 파일을 가져올 수 있습니다. Varonis Threat Labs의 연구원들은 SearchLeak이라고 하는 원클릭 유출 경로에 3개의 버그를 연결했습니다. 링크가 실제 microsoft.com 도메인을 가리키기 때문에 기존의 피싱 방지 및 URL 필터링 도구에서는 해당 도메인에 플래그를 지정할 가능성이 없습니다. 메시지도 없고, 비밀번호도 없고, 두 번째 클릭도 없습니다. Microsoft는 CVE-2026-42824를 할당하고 중요로 표시했습니다. CVSS 점수는 Microsoft에서 6.5점, National Vulnerability Database에서 7.5점으로 더 낮았고 동의하지 않았습니다. 회사는 백엔드의 결함을 완화했기 때문에 고객은 걱정할 필요가 없으며 Varonis는 관찰된 악용이 아닌 개념 증명을 제시했습니다. Microsoft의 권고에서는 이 결함을 네트워크를 통해 정보를 노출할 수 있는 명령 주입으로 설명합니다. 실제로 SearchLeak은 두 개의 오래된 웹 버그에 하나의 AI 관련 약점을 누적하고 각 링크는 다음 버그에 필요합니다. 진입점은 Copilot Enterprise 검색 URL의 q 매개 변수입니다. 이는 자연어 쿼리를 위한 것이지만 Copilot은 검색 문자열뿐만 아니라 지침으로 거기에 있는 모든 것을 읽습니다.