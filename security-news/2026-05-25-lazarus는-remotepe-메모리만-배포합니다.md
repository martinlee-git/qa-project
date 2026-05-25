# Lazarus는 Remotepe 메모리만 배포합니다.
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/05/lazarus-deploys-remotepe-memory-only.html
- Published At: unknown
- Collected At: 2026-05-25T22:09:05.882Z
- Notion Page: https://www.notion.so/The-Hacker-News-Lazarus-Remotepe-36bfc93aec578102aea9e9c0b001c280
- Original Title: Lazarus Deploys Remotepe Memory Only
## Summary
Lazarus는 메모리 전용 악성 코드를 사용하여 암호화 회사에 대해 RemotePE를 배포하여 은밀하고 장기적인 금융 침입을 가능하게 했습니다. 사이버 보안 연구원들이 북한과 연계된 Lazarus Group이 금융 및 암호화폐 조직을 표적으로 삼는 공격에 사용했던 RemotePE라는 크로스 플랫폼 악성 코드를 밝혀냈습니다. NCC 그룹 자회사 Fox-IT의 RemotePE는 DPAPILoader 및 RemotePELoader로 추적되는 두 개의 로더를 포함하는 다단계 공격 체인의 일부입니다. 보안 연구원인 Yun Zheng Hu와 Mick Koomen은 "DPAPILoader는 Windows 데이터 보호 API(DPAPI)를 사용하여 디스크에서 RemotePELoader를 해독하고 로드합니다."라고 말했습니다. "RemotePELoader는 C2 서버에 비콘을 연결하고…

## Original Description

Lazarus deployed RemotePE against crypto firms using memory-only malware, enabling stealthy long-term financial intrusions.
## Key Points
- Lazarus는 메모리 전용 악성 코드를 사용하여 암호화 회사에 대해 RemotePE를 배포하여 은밀하고 장기적인 금융 침입을 가능하게 했습니다.
- 사이버 보안 연구원들이 북한과 연계된 Lazarus Group이 금융 및 암호화폐 조직을 표적으로 삼는 공격에 사용했던 RemotePE라는 크로스 플랫폼 악성 코드를 밝혀냈습니다.
- NCC 그룹 자회사 Fox-IT의 RemotePE는 DPAPILoader 및 RemotePELoader로 추적되는 두 개의 로더를 포함하는 다단계 공격 체인의 일부입니다.
## Excerpt
사이버 보안 연구원들이 북한과 연계된 Lazarus Group이 금융 및 암호화폐 조직을 표적으로 삼는 공격에 사용했던 RemotePE라는 크로스 플랫폼 악성 코드를 밝혀냈습니다. NCC 그룹 자회사 Fox-IT의 RemotePE는 DPAPILoader 및 RemotePELoader로 추적되는 두 개의 로더를 포함하는 다단계 공격 체인의 일부입니다. 보안 연구원인 Yun Zheng Hu와 Mick Koomen은 "DPAPILoader는 Windows 데이터 보호 API(DPAPI)를 사용하여 디스크에서 RemotePELoader를 해독하고 로드합니다."라고 말했습니다. "RemotePELoader는 C2 서버에 신호를 보내고 다음 단계인 RemotePE를 수신할 때까지 기다립니다. RAT는 메모리에서 완전히 실행되고 디스크에 기록되지 않아 파일 시스템 아티팩트를 남기지 않습니다." RemotePE는 탈중앙화 금융(DeFi) 부문의 이름 없는 조직을 표적으로 삼은 공격과 관련하여 2025년 9월 보안 공급업체에 의해 처음으로 주목받았으며, 이로 인해 PondRAT, ThemeForestRAT 및 RemotePE를 포함한 세 가지 악성 코드군이 배포되었습니다. 침입은 무역 회사의 기존 직원으로 가장하여 텔레그램에서 피해자에게 접근하고 가짜 Calendly 및 Picktime 도메인에서 회의 일정을 잡은 후 소셜 엔지니어링을 통해 직원의 장치를 손상시키면서 시작되었습니다.