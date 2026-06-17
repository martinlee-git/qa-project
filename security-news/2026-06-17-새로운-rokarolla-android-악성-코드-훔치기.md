# 새로운 Rokarolla Android 악성 코드 훔치기
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/new-rokarolla-android-malware-steals.html
- Published At: unknown
- Collected At: 2026-06-17T05:17:42.809Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Rokarolla-Android-381fc93aec578198bc92eaea3283beea
- Original Title: New Rokarolla Android Malware Steals
## Summary
Rokarolla는 137개의 명령으로 217개의 은행 및 암호화폐 앱을 표적으로 삼아 PIN, SMS 코드, 암호화폐 결제 도난을 가능하게 합니다. Zimperium의 zLabs 보안 연구원들은 217개의 뱅킹 및 암호화폐 앱을 표적으로 삼고 137개의 원격 명령을 포함하는 새로운 Android 뱅킹 트로이 목마인 Rokarolla를 문서화했습니다. 이를 통해 운영자는 감염된 휴대폰을 거의 완벽하게 제어할 수 있습니다. 잠금 화면 PIN을 해제하고, SMS를 읽고 보내고, 클립보드를 다시 작성하여 암호화폐 결제를 리디렉션하고, Google Play 프로텍트를 끄는 등의 작업을 수행합니다. 명령 및 제어 서버의 이름을 딴 Rokarolla는 TikTok 및 Chrome과 같이 잘 알려진 앱으로 가장하는 악성 웹사이트를 통해 확산됩니다. 피해자가 가장 먼저 설치하는 것은 드로퍼(dropper)다.

## Original Description

Rokarolla targets 217 banking and crypto apps with 137 commands, enabling PIN, SMS code, and crypto payment theft.
## Key Points
- Rokarolla는 137개의 명령으로 217개의 은행 및 암호화폐 앱을 표적으로 삼아 PIN, SMS 코드, 암호화폐 결제 도난을 가능하게 합니다.
- Zimperium의 zLabs 보안 연구원들은 217개의 뱅킹 및 암호화폐 앱을 표적으로 삼고 137개의 원격 명령을 포함하는 새로운 Android 뱅킹 트로이 목마인 Rokarolla를 문서화했습니다.
- 이를 통해 운영자는 감염된 휴대폰을 거의 완벽하게 제어할 수 있습니다. 잠금 화면 PIN을 해제하고, SMS를 읽고 보내고, 클립보드를 다시 작성하여 암호화폐 결제를 리디렉션하고, Google Play 프로텍트를 끄는 등의 작업을 수행합니다.
## Excerpt
Zimperium의 zLabs 보안 연구원들은 217개의 뱅킹 및 암호화폐 앱을 표적으로 삼고 137개의 원격 명령을 포함하는 새로운 Android 뱅킹 트로이 목마인 Rokarolla를 문서화했습니다. 이를 통해 운영자는 감염된 휴대폰을 거의 완벽하게 제어할 수 있습니다. 잠금 화면 PIN을 해제하고, SMS를 읽고 보내고, 클립보드를 다시 작성하여 암호화폐 결제를 리디렉션하고, Google Play 프로텍트를 끄는 등의 작업을 수행합니다. 명령 및 제어 서버의 이름을 딴 Rokarolla는 TikTok 및 Chrome과 같이 잘 알려진 앱으로 가장하는 악성 웹사이트를 통해 확산됩니다. 피해자가 가장 먼저 설치하는 것은 Google Play Protect인 것처럼 가장하는 드로퍼입니다. 해당 변장을 사용하여 페이로드를 설치하고 접근성 액세스 권한을 얻습니다. 맬웨어가 실행되면 해당 명령 중 하나가 Play Protect를 끕니다. 도난은 오버레이를 통해 진행됩니다. Rokarolla는 서버에서 대상 목록을 가져와 활성 플래그가 지정된 각 앱에 대해 가짜 HTML 로그인 페이지를 다운로드하여 로컬 데이터베이스에 저장합니다. 피해자가 실제 은행 앱이나 지갑 앱을 열면 악성코드는 가짜 페이지를 맨 위에 놓고 카드 세부정보를 포함해 거기에 입력된 모든 내용을 캡처합니다.