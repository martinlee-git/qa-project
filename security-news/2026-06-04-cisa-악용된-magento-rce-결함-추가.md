# Cisa, 악용된 Magento Rce 결함 추가
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/cisa-adds-exploited-magento-rce-flaw.html
- Published At: unknown
- Collected At: 2026-06-04T11:47:58.227Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Cisa-Magento-Rce-375fc93aec578187af00cccd754b4003
- Original Title: Cisa Adds Exploited Magento Rce Flaw
## Summary
CISA는 적극적으로 악용된 후 Magento 매장에 영향을 미치는 CVSS 9.8 Mirasvit Cache Warmer 결함인 CVE-2026-45247을 KEV 카탈로그에 추가했습니다. 미국 사이버 보안 및 인프라 보안국(CISA)은 인기 있는 Magento 전체 페이지 캐시 확장 프로그램인 Mirasvit Cache Warmer에 영향을 미치는 치명적인 결함을 알려진 악용 취약점(KEV) 카탈로그에 추가했습니다. CVE-2026-45247(CVSS 점수: 9.8)로 추적되는 이 취약점은 영향을 받는 서버에서 임의의 PHP 코드를 실행하는 데 악용될 수 있는 신뢰할 수 없는 데이터의 역직렬화 사례입니다. "Mirasvit Full Page Cache Warmer에는 신뢰할 수 없는 데이터 취약점의 역직렬화가 포함되어 있습니다…

## Original Description

CISA added CVE-2026-45247, a CVSS 9.8 Mirasvit Cache Warmer flaw affecting Magento stores, to its KEV catalog after active exploitation.
## Key Points
- CISA는 적극적으로 악용된 후 Magento 매장에 영향을 미치는 CVSS 9.8 Mirasvit Cache Warmer 결함인 CVE-2026-45247을 KEV 카탈로그에 추가했습니다.
- 미국
- CISA(사이버보안 및 인프라 보안국)는 수요일, 널리 사용되는 Magento 전체 페이지 캐시 확장 프로그램인 Mirasvit Cache Warmer에 영향을 미치는 치명적인 결함을 알려진 악용 취약점(KEV) 카탈로그에 추가했습니다.
## Excerpt
미국 사이버 보안 및 인프라 보안국(CISA)은 인기 있는 Magento 전체 페이지 캐시 확장 프로그램인 Mirasvit Cache Warmer에 영향을 미치는 치명적인 결함을 알려진 악용 취약점(KEV) 카탈로그에 추가했습니다. CVE-2026-45247(CVSS 점수: 9.8)로 추적되는 이 취약점은 영향을 받는 서버에서 임의의 PHP 코드를 실행하는 데 악용될 수 있는 신뢰할 수 없는 데이터의 역직렬화 사례입니다. CISA는 "Mirasvit Full Page Cache Warmer에는 인증되지 않은 공격자가 CacheWarmer 쿠키에 조작된 직렬화된 PHP 개체를 제공하여 원격 코드 실행을 달성할 수 있도록 허용할 수 있는 신뢰할 수 없는 데이터 취약점의 역직렬화가 포함되어 있습니다"라고 밝혔습니다. 이 단점은 버전 1.11.12 이전의 모든 확장 버전에 영향을 미칩니다. 패치는 2026년 5월 25일에 출시되었습니다. KEV 카탈로그에 CVE-2026-45247이 추가된 것은 Sansec이 PHP 개체 주입 취약점이 제작된 CacheWarmer 쿠키를 전달하는 모든 상점 요청을 통해 악용될 수 있다고 말한 지 며칠 후에 나온 것입니다. 그런 다음 인증이나 관리자 권한을 요구하지 않고 PHP의 기본 unserialize() 기능을 사용하여 쿠키 값의 일부를 역직렬화합니다.