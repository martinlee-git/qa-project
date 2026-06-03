# Gamaredon은 Winrar를 이용하여 배달합니다.
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/gamaredon-exploits-winrar-to-deliver.html
- Published At: unknown
- Collected At: 2026-06-03T08:28:56.065Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Gamaredon-Winrar-373fc93aec57814cae85d86b8d374421
- Original Title: Gamaredon Exploits Winrar To Deliver
## Summary
Gamaredon은 2026년 1월 간첩 캠페인에서 GammaPhish와 GammaWorm을 사용하여 우크라이나 전역에서 은밀한 지속성과 데이터 도난을 가능하게 했습니다. Gamaredon으로 알려진 러시아 해킹 그룹은 데이터 절도 및 전파를 목표로 하는 여러 악성 코드군을 전달하기 위해 WinRAR 취약점을 지속적으로 악용한 것으로 알려져 있습니다. Sekoia에 따르면 이 활동에는 WinRAR의 경로 탐색 결함인 CVE-2025-8088을 무기화하여 GammaPhish라는 HTML 애플리케이션 페이로드를 실행한 다음 코드명 GammaLoad라는 중간 Visual Basic Script(VBScript) 다운로더를 검색하는 데 사용됩니다. 감염 체인은 2026년 1월 프랑스 사이버 보안 회사에 의해 관찰되었습니다. "그들의…

## Original Description

Gamaredon used GammaPhish and GammaWorm in a January 2026 espionage campaign, enabling stealthy persistence and data theft across Ukraine.
## Key Points
- Gamaredon은 2026년 1월 간첩 캠페인에서 GammaPhish와 GammaWorm을 사용하여 우크라이나 전역에서 은밀한 지속성과 데이터 도난을 가능하게 했습니다.
- Gamaredon으로 알려진 러시아 해킹 그룹은 데이터 절도 및 전파를 목표로 하는 여러 악성 코드군을 전달하기 위해 WinRAR 취약점을 지속적으로 악용한 것으로 알려져 있습니다.
- Sekoia에 따르면 이 활동에는 WinRAR의 경로 탐색 결함인 CVE-2025-8088을 무기화하여 GammaPhish라는 HTML 애플리케이션 페이로드를 실행한 다음 코드명 GammaLoad라는 중간 Visual Basic Script(VBScript) 다운로더를 검색하는 데 사용됩니다.
## Excerpt
Gamaredon으로 알려진 러시아 해킹 그룹은 데이터 절도 및 전파를 목표로 하는 여러 악성 코드군을 전달하기 위해 WinRAR 취약점을 지속적으로 악용한 것으로 알려져 있습니다. Sekoia에 따르면 이 활동에는 WinRAR의 경로 탐색 결함인 CVE-2025-8088을 무기화하여 GammaPhish라는 HTML 애플리케이션 페이로드를 실행한 다음 코드명 GammaLoad라는 중간 Visual Basic Script(VBScript) 다운로더를 검색하는 데 사용됩니다. 감염 체인은 2026년 1월 프랑스 사이버 보안 회사에 의해 관찰되었습니다. Sekoia는 "그들의 주요 목표는 호스트 시스템을 지문으로 식별하고, DDR(Dead Drop Resolver)을 사용하여 레지스트리의 네트워크 구성을 업데이트하고, C2 서버에서 임의의 VBScript 페이로드를 가져와 실행하는 것"이라고 말했습니다. 페이로드 중 하나는 예약된 작업을 통해 지속성을 설정하고 네트워크 공유 및 USB 드라이브의 합법적인 디렉터리를 숨기고 악성 Windows 바로 가기(LNK) 파일로 대체하여 명령 및 제어(C2) 서버에서 검색된 임의 코드를 실행하도록 설계된 GammaWorm이라는 VBScript 웜입니다. C2를 해결하기 위해 GammaWorm은 하드 코딩된 공개 텔레그램 채널에 대한 컬을 통해 GET 요청을 시작합니다. Telegram과 같은 합법적인 플랫폼을 사용하여 일반 트래픽과 혼합하고 탐지를 피하며 장기적인 간첩 활동을 유지하려는 아이디어입니다. GammaWorm은 또한 핵심 모듈을 숨기기 위해 NTFS 대체 데이터 스트림(ADS) 기술을 사용합니다.