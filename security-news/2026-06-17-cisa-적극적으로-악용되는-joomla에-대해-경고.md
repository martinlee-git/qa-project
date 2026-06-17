# Cisa, 적극적으로 악용되는 Joomla에 대해 경고
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/cisa-warns-of-actively-exploited-joomla.html
- Published At: unknown
- Collected At: 2026-06-17T09:20:40.211Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Cisa-Joomla-382fc93aec578135a7bce0428fecf45d
- Original Title: Cisa Warns Of Actively Exploited Joomla
## Summary
CISA는 적극적으로 악용된 후 Joomla JCE의 CVE-2026-48907을 KEV 카탈로그에 추가했습니다. 수정 사항은 6월 19일까지 마감됩니다. 미국 CISA(사이버보안 및 인프라 보안국)는 화요일 Widget Factory Joomla Content Editor(JCE)에 영향을 미치는 최대 심각도의 보안 결함을 KEV(알려진 악용 취약점) 카탈로그에 추가하여 활성 악용의 증거를 인용했습니다. CVE-2026-48907(CVSS 점수: 10.0)로 추적된 이 취약점은 임의 코드 실행을 용이하게 할 수 있는 부적절한 액세스 제어 사례입니다. "Widget Factory Joomla Content Editor에는 새로운 편집기 생성을 통해 PHP 코드를 업로드하고 실행할 수 있는 부적절한 액세스 제어 취약점이 포함되어 있습니다.…

## Original Description

CISA added CVE-2026-48907 in Joomla JCE to its KEV catalog after active exploitation; fixes are due by June 19.
## Key Points
- CISA는 적극적으로 악용된 후 Joomla JCE의 CVE-2026-48907을 KEV 카탈로그에 추가했습니다. 수정 사항은 6월 19일까지 완료됩니다.
- 미국
- CISA(사이버 보안 및 인프라 보안국)는 화요일에 활성 악용의 증거를 인용하면서 알려진 악용 취약점(KEV) 카탈로그에 Widget Factory Joomla Content Editor(JCE)에 영향을 미치는 최대 심각도의 보안 결함을 추가했습니다.
## Excerpt
미국 사이버 보안 및 인프라 보안국(CISA)은 화요일에 활발한 악용의 증거를 인용하면서 알려진 악용 취약점(KEV) 카탈로그에 Widget Factory Joomla Content Editor(JCE)에 영향을 미치는 최대 심각도의 보안 결함을 추가했습니다. CVE-2026-48907(CVSS 점수: 10.0)로 추적된 이 취약점은 임의 코드 실행을 용이하게 할 수 있는 부적절한 액세스 제어 사례입니다. CISA는 "Widget Factory Joomla Content Editor에는 인증되지 않은 사용자를 위한 새로운 편집기 프로필 생성을 통해 PHP 코드를 업로드하고 실행할 수 있는 부적절한 액세스 제어 취약점이 포함되어 있습니다"라고 밝혔습니다. CVE.org에 게시된 취약점에 대한 설명에 따르면, 이 문제는 Joomla용 JCE 편집기 확장에 존재하며, 악의적인 행위자가 인증되지 않은 사용자를 위한 새로운 편집기 프로필을 생성하여 효과적으로 PHP 코드 업로드 및 실행을 위한 길을 열 수 있습니다. 이 문제는 JCE 버전 1.0.0부터 2.9.99.4까지 영향을 미칩니다. 2026년 6월 3일에 출시된 버전 2.9.99.5에서 패치되었습니다. Widget Factory는 릴리스 노트에서 "부족한 액세스 제어로 인해 인증되지 않은 사용자가 편집자 프로필을 업로드할 수 있었습니다"라고 밝혔습니다.