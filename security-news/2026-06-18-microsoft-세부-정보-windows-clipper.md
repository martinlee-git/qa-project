# Microsoft 세부 정보 Windows Clipper
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/microsoft-details-windows-clipper.html
- Published At: unknown
- Collected At: 2026-06-18T21:46:45.127Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Microsoft-Windows-Clipper-383fc93aec5781f88ab2c7d09288eba3
- Original Title: Microsoft Details Windows Clipper
## Summary
Microsoft는 2026년 2월부터 USB 제공 LNK 파일과 Tor 기반 C2를 사용하여 클립보드 암호화 데이터를 훔치는 Windows 클리퍼 악성 코드 캠페인을 보고했습니다. 마이크로소프트는 2026년 2월부터 사용자를 대상으로 한 윈도우 기반 암호화폐 클리퍼 캠페인의 세부 사항을 공개했습니다. 마이크로소프트 디펜더 보안 연구 팀은 화요일 발표된 분석에서 "이 캠페인의 클리퍼는 Windows 스크립트 호스트와 ActiveX 기반 로직을 사용하여 번들 Tor 프록시를 실행하고 숨겨진 서비스 C2 [명령 및 제어] 서버를 폴링합니다"라고 밝혔습니다. "고주빈도의 클립보드 절도, 스크린샷 유출, 지갑 주소 대체 등을 수행합니다." "이 클리퍼의 실행은 주목할 만합니다...

## Original Description

Microsoft reports a Windows clipper malware campaign using USB-delivered LNK files and Tor-based C2 since Feb 2026, stealing clipboard crypto data.
## Key Points
- Microsoft는 2026년 2월부터 USB 제공 LNK 파일과 Tor 기반 C2를 사용하여 클립보드 암호화 데이터를 훔치는 Windows 클리퍼 악성 코드 캠페인을 보고했습니다.
- Microsoft는 2026년 2월부터 사용자를 대상으로 한 Windows 기반 암호화폐 클리퍼 캠페인의 세부 정보를 공개했습니다.
- 마이크로소프트 디펜더 보안 연구팀은 화요일 발표된 분석에서 "이 캠페인의 클리퍼는 Windows 스크립트 호스트와 ActiveX 기반 논리를 사용하여 번들 Tor 프록시를 실행하고 숨겨진 서비스 C2 [명령 및 제어] 서버를 폴링합니다"라고 밝혔습니다.
## Excerpt
마이크로소프트는 2026년 2월부터 사용자를 대상으로 한 윈도우 기반 암호화폐 클리퍼 캠페인의 세부 사항을 공개했습니다. 마이크로소프트 디펜더 보안 연구 팀은 화요일 발표된 분석에서 "이 캠페인의 클리퍼는 Windows 스크립트 호스트와 ActiveX 기반 로직을 사용하여 번들 Tor 프록시를 실행하고 숨겨진 서비스 C2 [명령 및 제어] 서버를 폴링합니다"라고 밝혔습니다. "고주빈도의 클립보드 절도, 스크린샷 유출, 지갑 주소 대체 등을 수행합니다." "이 클리퍼의 실행은 기존 설치 프로그램이나 노출된 IP 기반 C2 인프라에 의존하지 않기 때문에 주목할 만합니다. 대신 휴대용 Tor 클라이언트를 배포하고 로컬 SOCKS5 프록시를 통해 트래픽을 라우팅하며 데이터 절도와 원격 코드 실행을 혼합하여 재정적 동기가 있는 절도자를 가벼운 백도어로 전환합니다." 클리퍼(Clipper) 악성코드는 사용자의 클립보드를 은밀하게 모니터링해 단기 버퍼에 붙여넣은 민감한 데이터를 가로채는 악성 소프트웨어의 일종이다. 알려진 블록체인 주소 패턴과 일치하는 지갑 주소 문자열을 대체하여 암호화폐 거래를 자신이 통제하는 주소로 재라우팅함으로써 주로 암호화폐 거래를 목표로 합니다. 공격에는 USB 저장 장치를 통해 악성 Windows 바로 가기(LNK) 파일을 배포하는 방법이 포함됩니다. 이 파일을 열면 시스템이 이미 감염되었는지 확인하고 페이로드가 없는 경우에만 원격 서버에서 페이로드를 가져오는 웜 구성 요소가 실행됩니다. 배포된 두 번째 모듈은 수확하는 클리퍼입니다.ts를 사용하여 암호화폐 지갑 정보를 유출합니다.