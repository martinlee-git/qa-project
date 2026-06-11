# Shinyhunters는 Oracle Peoplesoft를 악용합니다.
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/shinyhunters-exploits-oracle-peoplesoft.html
- Published At: unknown
- Collected At: 2026-06-11T20:48:48.533Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Shinyhunters-Oracle-Peoplesoft-37cfc93aec57815fb975c38722430eed
- Original Title: Shinyhunters Exploits Oracle Peoplesoft
## Summary
Oracle PeopleSoft 제로데이 CVE-2026-35273은 Oracle의 6월 10일 권고 이전에 악용되어 데이터를 노출시키고 강탈 공격을 촉발했습니다. ShinyHunters 강탈 조직은 Oracle PeopleSoft의 패치되지 않은 결함을 악용하여 기업 시스템에 침입하여 데이터를 훔치고 비공개로 유지하기 위해 비용을 요구했습니다. 캠페인은 대학에 가장 큰 타격을 입혔습니다. Google의 Mandiant는 이를 UNC6240으로 추적하는 그룹에 기인하며 활동 날짜를 5월 27일부터 6월 9일 사이로 지정했습니다. Oracle은 6월 10일까지 권고 사항을 게시하지 않았으므로 해당 버그는 전체 기간 동안 제로데이였습니다. CVE-2026-35273 결함은 PeopleSoft Enterprise PeopleTools의 원격 코드 실행 버그로 10점 만점에 9.8점을 받았습니다. 로그인이나 사용자가 필요하지 않습니다.

## Original Description

Oracle PeopleSoft zero-day CVE-2026-35273 was exploited before Oracle's June 10 advisory, exposing data and triggering extortion attacks.
## Key Points
- Oracle PeopleSoft 제로데이 CVE-2026-35273은 Oracle의 6월 10일 권고 이전에 악용되어 데이터를 노출시키고 강탈 공격을 촉발했습니다.
- ShinyHunters 강탈 조직은 Oracle PeopleSoft의 패치되지 않은 결함을 악용하여 기업 시스템에 침입하여 데이터를 훔치고 비공개로 유지하기 위해 비용을 요구했습니다.
- 캠페인은 대학에 가장 큰 타격을 입혔습니다.
## Excerpt
ShinyHunters 강탈 조직은 Oracle PeopleSoft의 패치되지 않은 결함을 악용하여 기업 시스템에 침입하여 데이터를 훔치고 비공개로 유지하기 위해 비용을 요구했습니다. 캠페인은 대학에 가장 큰 타격을 입혔습니다. Google의 Mandiant는 이를 UNC6240으로 추적하는 그룹에 기인하며 활동 날짜를 5월 27일부터 6월 9일 사이로 지정했습니다. Oracle은 6월 10일까지 권고 사항을 게시하지 않았으므로 해당 버그는 전체 기간 동안 제로데이였습니다. CVE-2026-35273 결함은 PeopleSoft Enterprise PeopleTools의 원격 코드 실행 버그로 10점 만점에 9.8점을 받았습니다. 서버를 장악하려면 로그인이나 사용자 상호 작용이 필요하지 않으며 HTTP를 통한 네트워크 액세스만 필요합니다. 외부에서 연결할 수 있는 환경 관리 허브를 사용하여 PeopleSoft를 실행하는 경우 이것이 노출이며 즉각적인 조치는 해당 엔드포인트를 잠그는 것입니다. 취약점은 환경 관리 허브(PSEMHUB) 뒤에 있는 부분인 업데이트 환경 관리 구성 요소에 있습니다. Oracle은 PeopleTools 8.61 및 8.62를 영향을 받는 것으로 나열하고 이전의 지원되지 않는 버전도 취약할 수 있다고 말합니다. 이 보고서는 TrendAI Zero Day Initiative와 TrendAI Research의 연구원들에게 감사를 표합니다. Mandiant CTO Charles Carmakal은 이 버그가 실제로 악용되고 있음을 확인했습니다. 오라클은 악용을 목격했는지 여부를 밝히지 않았습니다. 해당 권고는 지원 로그인 뒤의 패치 가용성 문서를 가리키며 전체 수정 사항이 광범위하게 제공되는지 여부는 불분명합니다. 현재 지침은 완화에 중점을 두고 있습니다.