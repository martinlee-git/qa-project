# 강화된 표적 Fortigate 방화벽
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/fortibleed-targeted-fortigate-firewalls.html
- Published At: unknown
- Collected At: 2026-06-24T01:14:35.606Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Fortigate-388fc93aec578137bc15e8774f9403bc
- Original Title: Fortibleed Targeted Fortigate Firewalls
## Summary
FortiBleed는 1억 1천만 개가 넘는 자격 증명을 식별하는 스니퍼와 무차별 대입 파이프라인을 통해 430,000개의 FortiGate 방화벽을 표적으로 삼았습니다. 재정적 이득을 추구하는 러시아어를 사용하는 초기 액세스 브로커(IAB)는 전 세계적으로 430,000개가 넘는 FortiGate 방화벽을 표적으로 삼은 FortiBleed로 알려진 대규모 자격 증명 수집 작업의 배후에 있는 것으로 평가됩니다. 2026년 2월부터 활성화된 이 캠페인에는 자격 증명 목록 수집, 노출된 서비스 검색, 접근 가능한 시스템 무차별 공격, 손상된 방화벽에 맞춤형 스니퍼 배포가 포함됩니다. SOCRadar는 "이러한 스니퍼는 일단 배포되면 손상된 장치를 통과하는 트래픽에서 일반 텍스트와 해시된 자격 증명을 캡처합니다."라고 말했습니다.

## Original Description

FortiBleed targeted 430,000 FortiGate firewalls with sniffers and brute-force pipelines that identified over 110 million credentials.
## Key Points
- FortiBleed는 1억 1천만 개가 넘는 자격 증명을 식별하는 스니퍼와 무차별 대입 파이프라인을 통해 430,000개의 FortiGate 방화벽을 표적으로 삼았습니다.
- 재정적 이득을 추구하는 러시아어를 사용하는 초기 액세스 브로커(IAB)는 전 세계적으로 430,000개가 넘는 FortiGate 방화벽을 표적으로 삼은 FortiBleed로 알려진 대규모 자격 증명 수집 작업의 배후에 있는 것으로 평가됩니다.
- 2026년 2월부터 활성화된 이 캠페인에는 자격 증명 목록 수집, 노출된 서비스 검색, 접근 가능한 시스템 무차별 공격, 손상된 방화벽에 맞춤형 스니퍼 배포가 포함됩니다.
## Excerpt
재정적 이득을 추구하는 러시아어를 사용하는 초기 액세스 브로커(IAB)는 전 세계적으로 430,000개가 넘는 FortiGate 방화벽을 표적으로 삼은 FortiBleed로 알려진 대규모 자격 증명 수집 작업의 배후에 있는 것으로 평가됩니다. 2026년 2월부터 활성화된 이 캠페인에는 자격 증명 목록 수집, 노출된 서비스 검색, 접근 가능한 시스템 무차별 공격, 손상된 방화벽에 맞춤형 스니퍼 배포가 포함됩니다. SOCRadar는 새로운 보고서에서 "이러한 스니퍼는 일단 배포되면 손상된 장치를 통과하는 트래픽에서 일반 텍스트와 해시된 자격 증명을 캡처합니다"라고 밝혔습니다. 그런 다음 공격자는 Active Directory 도메인 및 기타 노출된 서비스에 대해 자격 증명을 크랙하고 검증하고 재사용합니다." 작업의 핵심은 FortiOS 내장 진단 명령인 스니퍼 패킷 진단을 활용하여 감염된 어플라이언스에서 인증 트래픽을 수동적으로 캡처하는 FortigateSniffer라는 Golang 기반 도구입니다. 이 도구는 24개 프로토콜의 트래픽을 모니터링하고, 인증 데이터를 구문 분석하고, 자격 증명을 추출하도록 설계되었습니다. 위협 행위자들은 일부 "작업 흐름의 일부"를 지원하기 위해 CyberStrike라고 불리는 오픈 소스 AI 기반 공격 보안 플랫폼의 도움을 구했을 가능성이 있는 것으로 의심됩니다. 흥미롭게도 CyberStrikeAI라는 또 다른 오픈 소스 프레임워크는 Amazon Threat Intelligence가 올해 초 노출한 FortiGate 장치를 표적으로 하는 또 다른 자동화된 대량 검색 캠페인과 관련하여 사용되었습니다.