# Cisa Flags Litespeed Cpanel 플러그인 결함
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/cisa-flags-litespeed-cpanel-plugin-flaw.html
- Published At: unknown
- Collected At: 2026-06-16T07:01:44.939Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Cisa-Flags-Litespeed-Cpanel-381fc93aec5781249696ee5653e49982
- Original Title: Cisa Flags Litespeed Cpanel Plugin Flaw
## Summary
CISA는 KEV에 CVE-2026-54420을 추가하여 연방 기관이 2026년 6월 18일까지 LiteSpeed cPanel 루트 에스컬레이션을 패치하도록 요구했습니다. 미국 CISA(사이버보안 및 인프라 보안국)는 LiteSpeed cPanel 플러그인에 영향을 미치는 보안 결함을 KEV(알려진 악용 취약점) 카탈로그에 추가했으며, FCEB(연방 민간 행정부) 기관은 6월까지 수정 사항을 적용해야 합니다. 문제의 취약점은 CVE-2026-54420(CVSS 점수: 8.5)이며, 이는 권한 상승 사례로 설명되었습니다. 이를 통해 FTP 또는 웹 셸 액세스 권한이 있는 사용자는 CloudLinux 또는 CageFS를 실행하는 공유 호스팅 서버의 루트로 권한을 에스컬레이션할 수 있습니다. "2.4.8 이전의 LiteSpeed ​​cPanel 플러그인(…

## Original Description

CISA added CVE-2026-54420 to KEV, requiring federal agencies to patch LiteSpeed cPanel root escalation by June 18, 2026.
## Key Points
- CISA는 KEV에 CVE-2026-54420을 추가하여 연방 기관이 2026년 6월 18일까지 LiteSpeed ​​cPanel 루트 에스컬레이션을 패치하도록 요구했습니다.
- 미국
- CISA(사이버보안 및 인프라 보안국)는 LiteSpeed ​​cPanel 플러그인에 영향을 미치는 보안 결함을 KEV(알려진 악용 취약점) 카탈로그에 추가했으며, FCEB(연방 민간 행정부) 기관은 2026년 6월 18일까지 수정 사항을 적용해야 합니다.
## Excerpt
미국 사이버보안 및 인프라 보안국(CISA)은 알려진 악용 취약점(KEV) 카탈로그에 LiteSpeed cPanel 플러그인에 영향을 미치는 보안 결함을 추가했으며, 이에 따라 FCEB(연방 민간 행정부) 기관은 2026년 6월 18일까지 수정 사항을 적용해야 합니다. 문제의 취약점은 CVE-2026-54420(CVSS 점수: 8.5)이며, 이는 특권 사례로 설명됩니다. 에스컬레이션. 이를 통해 FTP 또는 웹 셸 액세스 권한이 있는 사용자는 CloudLinux 또는 CageFS를 실행하는 공유 호스팅 서버의 루트로 권한을 에스컬레이션할 수 있습니다. CVE.org의 취약점에 대한 설명에 따르면 "2.4.8 이전의 LiteSpeed ​​cPanel 플러그인(5.3.2.0 이전의 LiteSpeed ​​WHM 플러그인에 배포됨)은 CloudLinux/CageFS를 실행하는 공유 호스팅 서버에서 FTP 또는 웹 셸 액세스 권한을 가진 사용자가 제공한 심볼릭 링크를 잘못 처리합니다." 현재 취약점이 실제로 어떻게 악용되고 있는지, 해당 공격이 성공했는지는 알 수 없지만 LiteSpeed는 사용자에게 아래 명령을 실행하여 서버가 영향을 받는지 확인하도록 촉구했습니다. grep 명령에 출력이 표시되지 않으면 서버가 문제의 영향을 받지 않았다는 의미입니다. 출력이 있는 경우 LiteSpeed는 오탐을 배제하기 위해 추가 표시기를 공유했습니다.