# 새로운 Oxloader Loader가 악성 코드를 사용함
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/new-oxloader-loader-uses-malicious.html
- Published At: unknown
- Collected At: 2026-06-22T19:54:34.135Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Oxloader-Loader-387fc93aec578108ae34eb30373f27b8
- Original Title: New Oxloader Loader Uses Malicious
## Summary
연구원들은 가짜 Node.js 광고, Storj 호스팅 페이로드 및 OXLOADER를 사용하여 CastleStealer를 배포하는 악성 광고 캠페인인 REF8372에 대해 자세히 설명합니다. 사이버 보안 연구원들은 이전에 보고되지 않은 OXLOADER라는 악성 코드 로더를 통해 CastleStealer를 전달하는 새로운 캠페인의 세부 정보를 공개했습니다. Elastic Security Labs에 따르면 이 캠페인은 악성 Google Ads를 악성코드 배포의 출발점으로 활용합니다. 증거에 따르면 독립 국가 연합(CIS) 지역에 위치한 시스템 감염을 방지하기 위한 명시적인 제외가 존재하기 때문에 위협 행위자가 러시아어를 사용하고 금전적인 동기를 갖고 있을 가능성이 높습니다. 캠페인의 코드명은 REF83입니다…

## Original Description

Researchers detail REF8372, a malvertising campaign using fake Node.js ads, Storj-hosted payloads, and OXLOADER to deploy CastleStealer.
## Key Points
- 연구원들은 가짜 Node.js 광고, Storj 호스팅 페이로드 및 OXLOADER를 사용하여 CastleStealer를 배포하는 악성 광고 캠페인인 REF8372에 대해 자세히 설명합니다.
- 사이버 보안 연구원들은 이전에 보고되지 않은 OXLOADER라는 악성 코드 로더를 통해 CastleStealer를 전달하는 새로운 캠페인의 세부 정보를 공개했습니다.
- Elastic Security Labs에 따르면 이 캠페인은 악성 Google Ads를 악성코드 배포의 출발점으로 활용합니다.
## Excerpt
사이버 보안 연구원들은 이전에 보고되지 않은 OXLOADER라는 악성 코드 로더를 통해 CastleStealer를 전달하는 새로운 캠페인의 세부 정보를 공개했습니다. Elastic Security Labs에 따르면 이 캠페인은 악성 Google Ads를 악성코드 배포의 출발점으로 활용합니다. 증거에 따르면 독립 국가 연합(CIS) 지역에 위치한 시스템 감염을 방지하기 위한 명시적인 제외가 존재하기 때문에 위협 행위자가 러시아어를 사용하고 금전적인 동기를 갖고 있을 가능성이 높습니다. 캠페인의 코드명은 REF8372입니다. 연구원 Daniel Stepanic과 Jia Yu Chan은 기술 분석에서 "로더는 여러 난독화 계층(제어 흐름 평면화, 불투명 조건자, 혼합 부울-산술), 자체 수정 암호 해독 스텁을 사용하고 Windows .reloc 섹션을 남용하여 쉘코드를 준비합니다."라고 말했습니다. 공격은 의심하지 않는 사용자가 Google과 같은 검색 엔진에 "lts version of node.js"와 같은 쿼리를 입력하여 이를 우크라이나에 기반을 둔 것으로 알려진 확인된 이름 "ВОЛОДИМИР ТЕРЕЩЕНКО"로 게시된 가짜 광고를 통해 노출되는 가짜 웹사이트("node-js[.]prentiva99[.]info")로 리디렉션할 때 시작됩니다. 광고주 계정이 실제 위협 행위자와 연결되어 있는지, 아니면 전면 계정인지, 구매한 ID인지는 현재로서는 알 수 없습니다. 광고 캠페인과 함께 광고주 계정이 2026년 5월 14일에 Google에서 삭제되었습니다.