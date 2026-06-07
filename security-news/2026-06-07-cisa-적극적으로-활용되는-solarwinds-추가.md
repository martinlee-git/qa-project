# Cisa, 적극적으로 활용되는 Solarwinds 추가
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/cisa-adds-actively-exploited-solarwinds.html
- Published At: unknown
- Collected At: 2026-06-07T16:41:53.813Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Cisa-Solarwinds-377fc93aec5781ef8cf8e96cf02131bb
- Original Title: Cisa Adds Actively Exploited Solarwinds
## Summary
CISA는 활발하게 악용되고 있다는 증거가 나타난 후 심각도가 높은 SolarWinds Serv-U DoS 결함인 CVE-2026-28318을 KEV 카탈로그에 추가했습니다. 미국 사이버 보안 및 인프라 보안국(CISA)은 활성 악용의 증거를 인용하면서 SolarWinds Serv-U 다중 프로토콜 파일 서버 소프트웨어에 영향을 미치는 심각도가 높은 보안 결함을 KEV(알려진 악용 취약점) 카탈로그에 추가했습니다. CVE-2026-28318(CVSS 점수: 7.5)로 추적되는 이 취약점은 특정 조건에서 서비스 충돌을 일으키는 서비스 거부(DoS) 버그입니다. CISA는 이를 DoS 상황을 초래하는 통제되지 않은 리소스 소비 취약점이라고 설명했습니다. "SolarWinds Serv-U는 특수한 영향을 받기 쉽습니다…

## Original Description

CISA added CVE-2026-28318, a high-severity SolarWinds Serv-U DoS flaw, to its KEV catalog after evidence of active exploitation.
## Key Points
- CISA는 활발하게 악용되고 있다는 증거가 나타난 후 심각도가 높은 SolarWinds Serv-U DoS 결함인 CVE-2026-28318을 KEV 카탈로그에 추가했습니다.
- 미국
- CISA(사이버보안 및 인프라 보안국)는 활성 악용의 증거를 인용하여 SolarWinds Serv-U 다중 프로토콜 파일 서버 소프트웨어에 영향을 미치는 심각도가 높은 보안 결함을 KEV(알려진 악용 취약점) 카탈로그에 추가했습니다.
## Excerpt
미국 사이버 보안 및 인프라 보안국(CISA)은 활성 악용의 증거를 인용하면서 SolarWinds Serv-U 다중 프로토콜 파일 서버 소프트웨어에 영향을 미치는 심각도가 높은 보안 결함을 KEV(알려진 악용 취약점) 카탈로그에 추가했습니다. CVE-2026-28318(CVSS 점수: 7.5)로 추적되는 이 취약점은 특정 조건에서 서비스 충돌을 일으키는 서비스 거부(DoS) 버그입니다. CISA는 이를 DoS 상황을 초래하는 통제되지 않은 리소스 소비 취약점이라고 설명했습니다. SolarWinds는 이번 주 초 발표한 권고에서 "SolarWinds Serv-U는 Content-Encoding: deflate를 사용하는 인증 없이 Serv-U 서비스를 중단시키는 특수 제작된 POST 요청에 취약합니다"라고 말했습니다. 이 문제는 SolarWinds Serv-U 버전 15.5.4 HF1에서 해결되었습니다. 완화 조치로서, 취약한 서비스에는 이 기능이 필요하지 않으므로 알려진 주소에 대한 액세스를 제한하고 "콘텐츠 인코딩"이 포함된 요청을 차단하는 것이 좋습니다. 현재 실제 공격에서 이 취약점이 어떻게 악용되고 있는지, 그 배후가 누구인지에 대한 세부 정보는 없습니다. 또한 인터넷에 노출된 Serv-U 인스턴스가 얼마나 많이 손상되었는지도 확실하지 않습니다.