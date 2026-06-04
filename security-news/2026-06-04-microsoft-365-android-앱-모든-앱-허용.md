# Microsoft 365 Android 앱 모든 앱 허용
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/microsoft-365-android-apps-let-any-app.html
- Published At: unknown
- Collected At: 2026-06-04T03:41:58.105Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Microsoft-365-Android-374fc93aec5781f1830ec63175c42295
- Original Title: Microsoft 365 Android Apps Let Any App
## Summary
디버그 플래그는 Microsoft 365 Android 토큰 확인을 비활성화하여 신뢰할 수 없는 앱이 계정에 액세스하도록 허용합니다. 위험을 줄이기 위해 5월 12일에 발표된 패치 여러 Microsoft 365 Android 앱의 프로덕션 빌드에서 개발 플래그가 켜진 상태로 유지되어 계정 토큰 공유를 신뢰할 수 있는 Microsoft 앱으로 제한하는 검사가 비활성화되었습니다. 동일한 휴대폰에 있는 다른 앱은 로그인한 사용자의 토큰을 요청하여 토큰을 얻은 다음 해당 사용자로서 이메일을 읽고, 파일을 열고, 캘린더를 탐색하고, 메시지를 보낼 수 있습니다. 비밀번호도 없고, 로그인 화면도 없고, 권한 메시지도 없습니다. Microsoft는 이를 패치했으며, Android에서 Microsoft 365 앱을 실행하는 경우 업데이트하세요. Enclave가 FlagLeft라고 부르는 이 버그는 Word, PowerPoint, Excel, Microsoft 365 Copi…

## Original Description

Debug flag disabled Microsoft 365 Android token checks, letting untrusted apps access accounts; patches issued May 12 to reduce risk
## Key Points
- 디버그 플래그는 Microsoft 365 Android 토큰 확인을 비활성화하여 신뢰할 수 없는 앱이 계정에 액세스하도록 허용합니다. 위험을 줄이기 위해 5월 12일에 발표된 패치 여러 Microsoft 365 Android 앱의 프로덕션 빌드에서 개발 플래그가 켜진 상태로 유지되어 계정 토큰 공유를 신뢰할 수 있는 Microsoft 앱으로 제한하는 검사가 비활성화되었습니다.
- 동일한 휴대폰에 있는 다른 앱은 로그인한 사용자의 토큰을 요청하여 토큰을 얻은 다음 해당 사용자로서 이메일을 읽고, 파일을 열고, 캘린더를 탐색하고, 메시지를 보낼 수 있습니다.
- 비밀번호도 없고, 로그인 화면도 없고, 권한 메시지도 없습니다.
## Excerpt
여러 Microsoft 365 Android 앱의 프로덕션 빌드에서 개발 플래그가 켜진 채로 남아 있어 계정 토큰 공유를 신뢰할 수 있는 Microsoft 앱으로 제한하는 확인이 비활성화되었습니다. 동일한 휴대폰에 있는 다른 앱은 로그인한 사용자의 토큰을 요청하여 토큰을 얻은 다음 해당 사용자로서 이메일을 읽고, 파일을 열고, 캘린더를 탐색하고, 메시지를 보낼 수 있습니다. 비밀번호도 없고, 로그인 화면도 없고, 권한 메시지도 없습니다. Microsoft는 이를 패치했으며, Android에서 Microsoft 365 앱을 실행하는 경우 업데이트하세요. Enclave가 FlagLeft라고 부르는 이 버그는 Word, PowerPoint, Excel, Microsoft 365 Copilot, Microsoft Loop 및 OneNote 등 6개 앱에 수십억 건의 다운로드가 발생했습니다. 동일한 플래그가 false로 설정된 상태로 배송된 팀은 영향을 받지 않았습니다. Enclave는 이를 설계가 아닌 전표로 읽습니다. Microsoft 365 앱은 의도적으로 계정 액세스를 공유하므로 Word에 로그인하면 PowerPoint에 다시 로그인하지 않아도 됩니다. 핸드오프는 누가 요청하는지 확인하고 신뢰할 수 있는 Microsoft 앱이 아닌 것은 거부하도록 되어 있습니다.