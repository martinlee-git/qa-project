# 중요한 Wp Maps Pro 결함이 적극적으로 발생함
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/critical-wp-maps-pro-flaw-actively.html
- Published At: unknown
- Collected At: 2026-06-01T12:59:59.776Z
- Notion Page: https://www.notion.so/The-Hacker-News-Wp-Maps-Pro-372fc93aec578166aa39d750a0108dd5
- Original Title: Critical Wp Maps Pro Flaw Actively
## Summary
CVE-2026-8732를 통해 공격자는 WP Maps Pro에서 관리자 계정을 만들 수 있습니다. 24시간 동안 2,858건의 공격이 취약한 사이트를 공격하여 탈취 위험이 있습니다. 위협 행위자들은 Envato Market에서 15,000개 이상의 매출을 올린 WordPress 플러그인인 WP Maps Pro에 영향을 미치는 심각한 보안 결함을 적극적으로 악용하여 취약한 사이트에 악성 관리자 계정을 생성하려고 시도하고 있습니다. WP Maps Pro를 사용하면 사이트 소유자가 WordPress 사이트에 마커, 목록 및 고급 위치 기능과 함께 사용자 정의 가능한 Google 지도 및 OpenStreetMap을 삽입할 수 있습니다. 이는 매장 찾기 도구로 사용되어 사용자가 인근 위치를 쉽게 찾고, 목록 세부정보를 보고, 길을 찾을 수 있도록 해줍니다. 문제의 취약점은 CVE-2026-…

## Original Description

CVE-2026-8732 lets attackers create admin accounts in WP Maps Pro; 2,858 attacks hit vulnerable sites in 24 hours, risking takeover.
## Key Points
- CVE-2026-8732를 통해 공격자는 WP Maps Pro에서 관리자 계정을 만들 수 있습니다. 24시간 동안 2,858건의 공격이 취약한 사이트를 공격하여 탈취 위험이 있습니다.
- 위협 행위자들은 Envato Market에서 15,000개 이상의 매출을 올린 WordPress 플러그인인 WP Maps Pro에 영향을 미치는 심각한 보안 결함을 적극적으로 악용하여 취약한 사이트에 악성 관리자 계정을 생성하려고 시도하고 있습니다.
- WP Maps Pro를 사용하면 사이트 소유자가 WordPress 사이트에 마커, 목록 및 고급 위치 기능과 함께 사용자 정의 가능한 Google 지도 및 OpenStreetMap을 삽입할 수 있습니다.
## Excerpt
위협 행위자들은 Envato Market에서 15,000개 이상의 매출을 올린 WordPress 플러그인인 WP Maps Pro에 영향을 미치는 심각한 보안 결함을 적극적으로 악용하여 취약한 사이트에 악성 관리자 계정을 생성하려고 시도하고 있습니다. WP Maps Pro를 사용하면 사이트 소유자가 WordPress 사이트에 마커, 목록 및 고급 위치 기능과 함께 사용자 정의 가능한 Google 지도 및 OpenStreetMap을 삽입할 수 있습니다. 이는 매장 찾기 도구로 사용되어 사용자가 인근 위치를 쉽게 찾고, 목록 세부정보를 보고, 길을 찾을 수 있도록 해줍니다. 문제의 취약점은 CVE-2026-8732(CVSS 점수: 9.8)로, 인증되지 않은 공격자가 관리 권한이 있는 WordPress 사용자를 생성하여 효과적으로 사이트를 제어할 수 있도록 허용하는 권한 상승 버그입니다. 단점은 6.1.0을 포함하여 이전 플러그인의 모든 버전에 영향을 미칩니다. 이 문제는 버전 6.1.1에서 해결되었습니다. 보안 연구원인 David Brown은 이 결함을 발견하고 보고한 공로를 인정 받았습니다. 높은 수준에서 문제는 문제 해결 중에 지원 직원이 고객 사이트에 로그인할 수 있도록 설계된 "임시 액세스" 기능에 뿌리를 두고 있습니다. 이 프로세스를 통해 인증되지 않은 사용자는 적절한 확인 없이 "wpgmp_temp_access_support()" 함수를 호출할 수 있으므로 궁극적으로 관리자 사용자를 생성할 수 있습니다.