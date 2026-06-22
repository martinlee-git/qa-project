# 해커들이 Gravity SMTP Wordpress를 악용했습니다.
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/hackers-exploit-gravity-smtp-wordpress.html
- Published At: unknown
- Collected At: 2026-06-22T05:43:37.970Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Gravity-SMTP-Wordpress-385fc93aec578179825ac95056a49f7a
- Original Title: Hackers Exploit Gravity Smtp Wordpress
## Summary
공격자들은 Gravity SMTP의 CVE-2026-4020을 악용하여 WordPress 사이트에서 API 키, OAuth 토큰 및 시스템 데이터를 유출하고 있습니다. 위협 행위자들은 약 100,000개 사이트에 설치된 WordPress 플러그인인 Gravity SMTP에 영향을 미치는 최근 패치된 보안 결함을 악용하고 있습니다. CVE-2026-4020(CVSS 점수: 5.3)으로 추적되는 이 취약점은 인증되지 않은 공격자가 플러그인의 이메일 통합을 위해 구성된 구성 데이터, API 키, 비밀 및 OAuth 토큰과 같은 민감한 데이터를 추출할 수 있는 중간 심각도의 정보 공개 결함입니다. "이는 무조건적으로 허용되는 허가 콜백을 사용하여 /wp-json/gravitysmtp/v1/tests/mock-data에 등록된 REST API 엔드포인트 때문입니다.

## Original Description

Attackers are exploiting CVE-2026-4020 in Gravity SMTP to leak API keys, OAuth tokens, and system data from WordPress sites.
## Key Points
- 공격자들은 Gravity SMTP의 CVE-2026-4020을 악용하여 WordPress 사이트에서 API 키, OAuth 토큰 및 시스템 데이터를 유출하고 있습니다.
- 위협 행위자들은 약 100,000개 사이트에 설치된 WordPress 플러그인인 Gravity SMTP에 영향을 미치는 최근 패치된 보안 결함을 악용하고 있습니다.
- CVE-2026-4020(CVSS 점수: 5.3)으로 추적되는 이 취약점은 인증되지 않은 공격자가 플러그인의 이메일 통합을 위해 구성된 구성 데이터, API 키, 비밀 및 OAuth 토큰과 같은 민감한 데이터를 추출할 수 있는 중간 심각도의 정보 공개 결함입니다.
## Excerpt
위협 행위자들은 약 100,000개 사이트에 설치된 WordPress 플러그인인 Gravity SMTP에 영향을 미치는 최근 패치된 보안 결함을 악용하고 있습니다. CVE-2026-4020(CVSS 점수: 5.3)으로 추적되는 이 취약점은 인증되지 않은 공격자가 플러그인의 이메일 통합을 위해 구성된 구성 데이터, API 키, 비밀 및 OAuth 토큰과 같은 민감한 데이터를 추출할 수 있는 중간 심각도의 정보 공개 결함입니다. Wordfence는 "이는 /wp-json/gravitysmtp/v1/tests/mock-data에 등록된 REST API 엔드포인트와 무조건 true를 반환하는permission_callback으로 인해 인증되지 않은 방문자가 액세스할 수 있기 때문입니다"라고 말했습니다. "?page=gravitysmtp-settings 쿼리 매개변수가 추가되면 플러그인의 Register_connector_data() 메소드가 내부 커넥터 데이터를 채워 엔드포인트가 전체 시스템 보고서가 포함된 약 365KB의 JSON을 반환하게 됩니다." 결과적으로 인증되지 않은 공격자는 이 문제를 무기화하여 다음을 포함한 광범위한 정보를 검색할 수 있습니다.