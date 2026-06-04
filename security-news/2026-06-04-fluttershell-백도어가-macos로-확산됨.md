# Fluttershell 백도어가 Macos로 확산됨
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/fluttershell-backdoor-spreads-to-macos.html
- Published At: unknown
- Collected At: 2026-06-04T14:49:55.486Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Fluttershell-Macos-375fc93aec578106af60d87372126faf
- Original Title: Fluttershell Backdoor Spreads To Macos
## Summary
Operation FlutterBridge는 애드웨어 기능을 갖춘 Flutter 기반 백도어인 FlutterShell을 확산시키는 macOS 악성 광고 캠페인입니다. 사이버 보안 연구원들은 FlutterShell이라는 새로운 백도어를 확산시키는 Operation FlutterBridge라는 코드명 macOS 악성 광고 캠페인을 밝혀냈습니다. Palo Alto Networks Unit 42에 따르면 이 캠페인은 2025년 8월 말에 JSCoreRunner(일명 FileRipple)라고 불리는 이전에 보고된 활동 클러스터의 다음 단계라고 합니다. 두 공격 체인 뒤에 있는 사이버 범죄 그룹은 CL-CRI-1089라는 이름으로 추적되고 있습니다. 공격자는 최소 2023년부터 활동한 것으로 평가된다. "Flutter 프레임워크를 사용하여 구축된 FlutterShell은 대상을 감염시킵니다…

## Original Description

Operation FlutterBridge is a macOS malvertising campaign spreading FlutterShell, a Flutter-based backdoor with adware capabilities.
## Key Points
- Operation FlutterBridge는 애드웨어 기능을 갖춘 Flutter 기반 백도어인 FlutterShell을 확산시키는 macOS 악성 광고 캠페인입니다.
- 사이버 보안 연구원들은 FlutterShell이라는 새로운 백도어를 확산시키는 Operation FlutterBridge라는 코드명 macOS 악성 광고 캠페인을 밝혀냈습니다.
- Palo Alto Networks Unit 42에 따르면 이 캠페인은 2025년 8월 말에 이전에 보고된 JSCoreRunner(일명 FileRipple)라는 활동 클러스터의 다음 단계라고 합니다.
## Excerpt
사이버 보안 연구원들은 FlutterShell이라는 새로운 백도어를 확산시키는 Operation FlutterBridge라는 코드명 macOS 악성 광고 캠페인을 밝혀냈습니다. Palo Alto Networks Unit 42에 따르면 이 캠페인은 2025년 8월 말에 JSCoreRunner(일명 FileRipple)라고 불리는 이전에 보고된 활동 클러스터의 다음 단계라고 합니다. 두 공격 체인 뒤에 있는 사이버 범죄 그룹은 CL-CRI-1089라는 이름으로 추적되고 있습니다. 공격자는 적어도 2023년부터 활동한 것으로 평가됩니다. Unit 42는 "Flutter 프레임워크를 사용하여 구축된 FlutterShell은 악성 데스크톱 애플리케이션을 통해 대상을 애드웨어로 감염시킵니다"라고 말했습니다. "애드웨어 기능 외에도 페이로드에는 셸 명령 실행 및 파일 시스템 조작을 포함한 백도어 기능이 있습니다." CL-CRI-1089로 인한 작업에는 Recipe Lister 및 Calendaromatic도 포함됩니다. 두 가지 모두 TamperedChef(일명 EvilAI)로 알려진 광범위한 명칭에 속하며, 트로이 목마 버전의 생산성 소프트웨어를 사용하여 잠재적으로 원치 않는 프로그램(PUP) 및 애드웨어를 전달하는 것과 관련된 지속적인 캠페인입니다. 이러한 캠페인은 Google이 인증한 셸 회사 네트워크를 사용하여 악성 Google 및 YouTube 광고를 배포하며, 이 광고는 대상을 속여 합법적인 데스크톱 애플리케이션으로 가장하는 악성 코드를 배포하도록 유도하는 역할을 합니다. 위장 회사 중 일부는 AdsParkPro LTD, Advantage Web Marketing LLC 및 SOFT WE ART LIMITED(현재 PACIFIC TRADE SOLUTIONS LTD)입니다.