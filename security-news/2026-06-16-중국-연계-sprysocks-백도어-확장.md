# 중국 연계 Sprysocks 백도어 확장
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/china-linked-sprysocks-backdoor-expands.html
- Published At: unknown
- Collected At: 2026-06-16T17:07:47.425Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Sprysocks-381fc93aec5781c6afb7c76335ce1686
- Original Title: China Linked Sprysocks Backdoor Expands
## Summary
ESET은 30개 이상의 명령이 포함된 두 가지 Windows SprySOCKS 변종, TCP를 통한 C2, UDP 및 WebSocket을 발견했으며 4개국의 정부 목표를 발견했습니다. 사이버 보안 연구원들은 SprySOCKS라고 불리는 Linux 전용 백도어로 간주되는 이전에 문서화되지 않은 두 가지 Windows 변종을 발견했습니다. ESET은 The Hacker News와 공유한 보고서에서 "발견된 Windows 변종은 내부적으로 WIN_DRV 및 WIN_PLUS로 표시되어 있습니다"라고 밝혔습니다. "두 가지 모두 하드 코딩된 C&C(명령 및 제어) 구성과 함께 제공되며 TCP, UDP 및 WebSocket 프로토콜을 통한 통신을 지원합니다." Linux 버전과 마찬가지로 Windows 버전은 시스템 정보 수집, 프로세스 열거 등을 용이하게 하기 위해 30개 이상의 명령을 지원합니다.

## Original Description

ESET found two Windows SprySOCKS variants with 30+ commands, C2 over TCP, UDP, and WebSocket, and government targets in 4 countries.
## Key Points
- ESET은 30개 이상의 명령이 포함된 두 가지 Windows SprySOCKS 변종, TCP를 통한 C2, UDP 및 WebSocket을 발견했으며 4개국의 정부 목표를 발견했습니다.
- 사이버 보안 연구원들은 SprySOCKS라고 불리는 Linux 전용 백도어로 간주되는 이전에 문서화되지 않은 두 가지 Windows 변종을 발견했습니다.
- ESET은 The Hacker News와 공유한 보고서에서 "발견된 Windows 변종은 내부적으로 WIN_DRV 및 WIN_PLUS로 표시되어 있습니다"라고 밝혔습니다.
## Excerpt
사이버 보안 연구원들은 SprySOCKS라고 불리는 Linux 전용 백도어로 간주되는 이전에 문서화되지 않은 두 가지 Windows 변종을 발견했습니다. ESET은 The Hacker News와 공유한 보고서에서 "발견된 Windows 변종은 내부적으로 WIN_DRV 및 WIN_PLUS로 표시되어 있습니다"라고 밝혔습니다. "두 가지 모두 하드 코딩된 C&C(명령 및 제어) 구성과 함께 제공되며 TCP, UDP 및 WebSocket 프로토콜을 통한 통신을 지원합니다." Linux 버전과 마찬가지로 Windows 버전은 시스템 정보 수집, 프로세스 열거, 서비스 관리 및 파일 시스템 작업을 용이하게 하는 30개 이상의 명령을 지원합니다. WIN_DRV는 또한 커널 드라이버를 활용하여 악성코드의 네트워크 연결, 프로세스, 파일 및 레지스트리 키를 숨기는 것으로 밝혀졌습니다. 또한, 이 변종은 악성코드 운영자가 네트워크 트래픽에서 백도어의 실제 수신 대기 포트를 노출시키지 않고 피해자 장치의 임의 TCP 포트를 통해 백도어로 명령을 보낼 수 있도록 하는 TCP 트래픽 전환을 가능하게 합니다. SprySOCKS는 2023년 9월 Trend Micro에 의해 처음으로 공개적으로 문서화되었으며, Earth Lusca로 알려진 중국 넥서스 국가 후원 위협 행위자가 이 공격을 사용했다는 사실이 밝혀졌습니다. 이 공격은 Aquatic Panda, Bronze University, Charcoal Typhoon 및 RedHotel이라는 이름으로 사이버 보안 커뮤니티에서도 추적됩니다. 해당 공격자는 최소 2021년부터 활동하고 있으며 아이순(i-Soon)이라는 중국 계약업체가 운영하는 것으로 평가된다.