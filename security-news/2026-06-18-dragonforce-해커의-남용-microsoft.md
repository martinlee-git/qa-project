# Dragonforce 해커의 남용 Microsoft
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/dragonforce-hackers-abuse-microsoft.html
- Published At: unknown
- Collected At: 2026-06-18T13:39:40.992Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Dragonforce-Microsoft-383fc93aec57818fbc57f101371c1c56
- Original Title: Dragonforce Hackers Abuse Microsoft
## Summary
DragonForce와 연결된 해커는 미국 회사의 공격 중에 Backdoor.Turn을 사용하여 Microsoft Teams 릴레이 인프라를 통해 C2 트래픽을 라우팅했습니다. DragonForce 랜섬웨어와 관련된 위협 행위자는 Microsoft Teams 릴레이 인프라 내부에 C2(명령 및 제어) 트래픽을 숨기기 위해 Backdoor.Turn이라는 사용자 지정 Go 기반 원격 액세스 트로이 목마(RAT)를 사용하는 것으로 관찰되었습니다. Broadcom이 소유한 Symantec과 Carbon Black의 조사 결과에 따르면 백도어는 미국의 주요 서비스 회사를 대상으로 배포되었습니다. 회사명은 공개되지 않았다. "Backdoor.Turn은 Microsoft의 Skype 지원 ID 서비스에서 익명의 Teams 방문자 토큰을 획득하고 합법적인 Microsoft TURN 릴레이를 사용합니다...

## Original Description

DragonForce-linked hackers used Backdoor.Turn to route C2 traffic through Microsoft Teams relay infrastructure during a U.S. firm attack.
## Key Points
- DragonForce와 연결된 해커는 Backdoor.Turn을 사용하여 미국에서 Microsoft Teams 릴레이 인프라를 통해 C2 트래픽을 라우팅했습니다.
- 확고한 공격.
- DragonForce 랜섬웨어와 관련된 위협 행위자는 Microsoft Teams 릴레이 인프라 내부에 C2(명령 및 제어) 트래픽을 숨기기 위해 Backdoor.Turn이라는 사용자 지정 Go 기반 원격 액세스 트로이 목마(RAT)를 사용하는 것으로 관찰되었습니다.
## Excerpt
DragonForce 랜섬웨어와 관련된 위협 행위자는 Microsoft Teams 릴레이 인프라 내부에 C2(명령 및 제어) 트래픽을 숨기기 위해 Backdoor.Turn이라는 사용자 지정 Go 기반 원격 액세스 트로이 목마(RAT)를 사용하는 것으로 관찰되었습니다. Broadcom이 소유한 Symantec과 Carbon Black의 조사 결과에 따르면 백도어는 미국의 주요 서비스 회사를 대상으로 배포되었습니다. 회사명은 공개되지 않았다. Threat Hunter Team은 The Hacker News와 공유한 보고서에서 "Backdoor.Turn은 Microsoft의 Skype 지원 ID 서비스에서 익명의 Teams 방문자 토큰을 획득하고 합법적인 Microsoft TURN 릴레이를 사용하여 연결을 설정한 다음 공격자의 실제 명령 및 제어(C2) 서버에 대한 QUIC 세션을 실행합니다"라고 밝혔습니다. "네트워크 방어자들이 볼 수 있는 유일한 트래픽은 합법적인 Microsoft Teams 서버에 대한 아웃바운드 연결이었습니다. 공격자들은 1~2개월 동안 피해자 네트워크에 있었습니다." 이번 개발은 Microsoft의 TURN(Traversal Using Relays around NAT) 릴레이 인프라를 악용하는 공격자가 공개적으로 문서화한 최초의 사례입니다.