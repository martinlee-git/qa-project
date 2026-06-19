# Apple 패치로 Studio Buds 결함 개선
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/apple-patches-beats-studio-buds-flaw.html
- Published At: unknown
- Collected At: 2026-06-19T13:55:41.739Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Apple-Studio-Buds-384fc93aec5781b49979f0f17557ac22
- Original Title: Apple Patches Beats Studio Buds Flaw
## Summary
Apple은 Beats Studio Buds 펌웨어 1B211의 CVE-2025-20701을 수정하여 Airoha SDK를 통해 근처에서 도청할 수 있는 Bluetooth 페어링 결함을 해결했습니다. Apple은 인근 해커가 사용자를 도청하기 위해 악용할 수 있는 심각도가 높은 취약점을 패치하기 위해 Beats Studio Buds 무선 이어버드를 업데이트했습니다. CVE-2025-20701(CVSS 점수: 8.8)로 추적되는 이 취약점은 사용자 동의 없이 Bluetooth 오디오 장치를 페어링할 수 있게 만드는 Airoha Bluetooth 오디오 SDK에 영향을 미치는 잘못된 인증 사례를 나타냅니다. 이 결함을 성공적으로 악용하면 추가 실행 권한이나 사용자 상호 작용 없이 권한이 원격으로 상승할 수 있습니다. 그만큼…

## Original Description

Apple fixed CVE-2025-20701 in Beats Studio Buds firmware 1B211, closing a Bluetooth pairing flaw that could allow nearby eavesdropping via Airoha SDK.
## Key Points
- Apple은 Beats Studio Buds 펌웨어 1B211의 CVE-2025-20701을 수정하여 Airoha SDK를 통해 근처에서 도청할 수 있는 Bluetooth 페어링 결함을 해결했습니다.
- Apple은 인근 해커가 사용자를 도청하기 위해 악용할 수 있는 심각도가 높은 취약점을 패치하기 위해 Beats Studio Buds 무선 이어버드를 업데이트했습니다.
- CVE-2025-20701(CVSS 점수: 8.8)로 추적되는 이 취약점은 사용자 동의 없이 Bluetooth 오디오 장치를 페어링할 수 있게 만드는 Airoha Bluetooth 오디오 SDK에 영향을 미치는 잘못된 인증 사례를 나타냅니다.
## Excerpt
Apple은 인근 해커가 사용자를 도청하기 위해 악용할 수 있는 심각도가 높은 취약점을 패치하기 위해 Beats Studio Buds 무선 이어버드를 업데이트했습니다. CVE-2025-20701(CVSS 점수: 8.8)로 추적되는 이 취약점은 사용자 동의 없이 Bluetooth 오디오 장치를 페어링할 수 있게 만드는 Airoha Bluetooth 오디오 SDK에 영향을 미치는 잘못된 인증 사례를 나타냅니다. 이 결함을 성공적으로 악용하면 추가 실행 권한이나 사용자 상호 작용 없이 권한이 원격으로 상승할 수 있습니다. 이 문제는 Beats 펌웨어 업데이트 1B211에서 해결되었습니다. Apple은 이번 주에 발표한 권고에서 "블루투스 범위 내의 공격자는 아직 페어링되지 않은 장치의 마이크를 통해 듣고 적극적으로 페어링 요청을 찾을 수 있습니다"라고 밝혔습니다. 이 취약점에 대한 자세한 내용은 ERNW GmbH 연구원인 Dennis Heinze와 Frieder Steinmetz가 독일에서 열린 TROOPERS 보안 컨퍼런스에서 Airoha SoC의 다른 두 가지 결함(CVE-2025-20700 및 CVE-2025-20702)과 함께 이를 표시하면서 2025년 6월에 처음 나타났습니다. 유사한 패치가 Jabra에서 2025년 12월에 출시되었습니다.