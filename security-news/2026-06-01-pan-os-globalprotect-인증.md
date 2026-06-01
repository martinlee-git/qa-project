# Pan Os Globalprotect 인증
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/05/pan-os-globalprotect-authentication.html
- Published At: unknown
- Collected At: 2026-06-01T00:50:59.946Z
- Notion Page: https://www.notion.so/The-Hacker-News-Pan-Os-Globalprotect-370fc93aec57813cb70ef91eea611115
- Original Title: Pan Os Globalprotect Authentication
## Summary
CVE-2026-0257은 2026년 5월 17일부터 PAN-OS 장치에서 활발히 악용되어 무단 VPN 액세스 및 네트워크 노출이 가능해졌습니다. Palo Alto Networks는 최근 공개된 PAN-OS 및 Prisma Access에 영향을 미치는 중간 심각도의 보안 결함이 실제로 활발하게 악용되고 있다고 경고했습니다. CVE-2026-0257(CVSS 점수: 7.8)로 추적되는 이 취약점은 악의적인 행위자가 VPN 연결을 설정하기 위해 악용할 수 있는 인증 우회 사례를 나타냅니다. "GlobalProtect 포털과 Palo Alto Networks PAN-OS® 소프트웨어의 게이트웨이에 있는 인증 우회 취약점으로 인해 공격자가 보안 제한을 우회하고 승인되지 않은 VPN 연결을 설정할 수 있습니다." Palo…

## Original Description

CVE-2026-0257 is being actively exploited on PAN-OS devices since May 17, 2026, enabling unauthorized VPN access and network exposure.
## Key Points
- CVE-2026-0257은 2026년 5월 17일부터 PAN-OS 장치에서 활발히 악용되어 무단 VPN 액세스 및 네트워크 노출이 가능해졌습니다.
- Palo Alto Networks는 최근 공개된 PAN-OS 및 Prisma Access에 영향을 미치는 중간 심각도의 보안 결함이 실제로 활발하게 악용되고 있다고 경고했습니다.
- CVE-2026-0257(CVSS 점수: 7.8)로 추적되는 이 취약점은 악의적인 행위자가 VPN 연결을 설정하기 위해 악용할 수 있는 인증 우회 사례를 나타냅니다.
## Excerpt
Palo Alto Networks는 최근 공개된 PAN-OS 및 Prisma Access에 영향을 미치는 중간 심각도의 보안 결함이 실제로 활발하게 악용되고 있다고 경고했습니다. CVE-2026-0257(CVSS 점수: 7.8)로 추적되는 이 취약점은 악의적인 행위자가 VPN 연결을 설정하기 위해 악용할 수 있는 인증 우회 사례를 나타냅니다. Palo Alto Networks는 2026년 5월 13일 발표된 권고에서 "GlobalProtect 포털 및 Palo Alto Networks PAN-OS® 소프트웨어의 게이트웨이에 있는 인증 우회 취약점을 통해 공격자가 보안 제한을 우회하고 승인되지 않은 VPN 연결을 설정할 수 있습니다."라고 Palo Alto Networks는 말했습니다. 이 문제는 특히 인증 무시 쿠키가 활성화되고 특정 인증서 구성이 존재할 때 구성된 GlobalProtect 포털 또는 게이트웨이가 있는 방화벽에 영향을 미친다고 네트워크 보안 회사는 말했습니다. Palo Alto Networks는 2026년 5월 29일 권고 업데이트에서 "완화 조치를 적용하지 않고 패치되지 않은 PAN-OS 장치에 대한 제한된 악용 시도를 인지하게 되었습니다."라고 밝혔습니다.