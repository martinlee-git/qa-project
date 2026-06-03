# 새로운 Google Doubleclick이 학대당했습니다.
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/google-doubleclick-abused-in-new.html
- Published At: unknown
- Collected At: 2026-06-03T20:36:56.711Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Google-Doubleclick-374fc93aec5781d3b2c3f78e318c73f2
- Original Title: Google Doubleclick Abused In New
## Summary
DoubleClick 리디렉션은 감지를 회피하고 호스트를 제어하기 위해 동적 미끼와 .NET 로더를 사용하여 DesckVB RAT 악성 스팸을 숨깁니다. 사이버 보안 연구원들은 탐지를 회피하고 궁극적으로 DesckVB RAT라는 원격 액세스 트로이 목마(RAT)를 전달하는 방법으로 Google의 DoubleClick 도메인을 사용하는 새로운 악성 스팸 캠페인을 표시했습니다. Huntress 연구원 Anna Pham과 Adam Mooney는 The Hacker News와 공유한 보고서에서 "피해자가 공격자가 제어하는 ​​인프라에 도달하기 전에 미끼는 많은 보안 도구가 의심스러운 것으로 간주할 가능성이 낮은 합법적인 Google 소유 도메인인 DoubleClick을 통해 경로를 지정합니다."라고 말했습니다. "여기서 피해자는 개인화된 악성 스팸 키트로 전달됩니다…

## Original Description

DoubleClick redirects hide DesckVB RAT malspam, using dynamic lures and .NET loaders to evade detection and control hosts.
## Key Points
- DoubleClick 리디렉션은 감지를 회피하고 호스트를 제어하기 위해 동적 미끼와 .NET 로더를 사용하여 DesckVB RAT 악성 스팸을 숨깁니다.
- 사이버 보안 연구원들은 탐지를 회피하고 궁극적으로 DesckVB RAT라는 원격 액세스 트로이 목마(RAT)를 전달하는 방법으로 Google의 DoubleClick 도메인을 사용하는 새로운 악성 스팸 캠페인을 표시했습니다.
- Huntress 연구원 Anna Pham과 Adam Mooney는 The Hacker News와 공유한 보고서에서 "피해자가 공격자가 제어하는 ​​인프라에 도달하기 전에 미끼는 많은 보안 도구가 의심스러운 것으로 간주할 가능성이 낮은 합법적인 Google 소유 도메인인 DoubleClick을 통해 경로를 지정합니다."라고 말했습니다.
## Excerpt
사이버 보안 연구원들은 탐지를 회피하고 궁극적으로 DesckVB RAT라는 원격 액세스 트로이 목마(RAT)를 전달하는 방법으로 Google의 DoubleClick 도메인을 사용하는 새로운 악성 스팸 캠페인을 표시했습니다. Huntress 연구원 Anna Pham과 Adam Mooney는 The Hacker News와 공유한 보고서에서 "피해자가 공격자가 제어하는 ​​인프라에 도달하기 전에 미끼는 많은 보안 도구가 의심스러운 것으로 간주할 가능성이 낮은 합법적인 Google 소유 도메인인 DoubleClick을 통해 경로를 지정합니다."라고 말했습니다. "여기서 피해자는 피해자의 이메일 주소를 사용하여 즉석에서 개인화되는 악성 스팸 키트로 전달되며, 운영자가 각 대상에 대한 미끼를 직접 제작할 필요 없이 페이지가 설득력 있게 느껴지도록 회사 브랜드 및 위치 세부 정보를 동적으로 끌어옵니다." 이 공격이 주목할 만한 이유는 각 대상 조직에 대해 맞춤형 키트를 보유할 필요가 없기 때문에 이러한 작업의 확장성과 비용 효율성이 향상된다는 것입니다. 캠페인의 최종 목표는 2026년 2월부터 활발하게 활동 중인 .NET 기반 트로이목마인 DesckVB RAT를 삭제하는 것입니다. 공격은 의심하지 않는 사용자가 피싱 이메일에 첨부된 HTML 파일을 열 때 시작됩니다. 파일은 Google DoubleClick Campaign Manager 클릭 추적 URL로의 메타 새로고침 브라우저 리디렉션을 트리거합니다. 여기서 사용자는 Base64로 인코딩된 이메일 주소를 디코딩하고 피해자를 "PDF 다운로드" 버튼이 포함된 랜딩 페이지로 연결하는 다른 리디렉터로 연결됩니다.