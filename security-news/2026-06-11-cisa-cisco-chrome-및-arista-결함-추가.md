# Cisa, Cisco Chrome 및 Arista 결함 추가
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/cisa-adds-cisco-chrome-and-arista-flaws.html
- Published At: unknown
- Collected At: 2026-06-11T05:39:50.351Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Cisa-Cisco-Chrome-Arista-37bfc93aec578165810fffd7fc449fd5
- Original Title: Cisa Adds Cisco Chrome And Arista Flaws
## Summary
CISA는 Cisco SD-WAN Manager, Chrome V8 및 Arista EOS에서 적극적으로 악용되는 결함 3개를 KEV 카탈로그에 추가했습니다. 미국 사이버보안 및 인프라 보안국(CISA)은 활성 악용이 보고된 후 화요일에 알려진 악용 취약점(KEV) 카탈로그에 세 가지 새로운 취약점을 추가했습니다. 취약점 목록은 다음과 같습니다. "VXLAN(Virtual Extensible LAN), 디캡 그룹 또는 GRE(Generic Routing Encapsulation) 터널 인터페이스와 같은 터널 캡슐화 해제 구성이 존재하는 Arista EOS를 실행하는 영향을 받는 플랫폼에서 스위치는 구성과 일치하는 대상 IP를 사용하여 예상치 못한 터널링된 패킷을 잘못 캡슐화 해제하고 전달합니다.

## Original Description

CISA added 3 actively exploited flaws in Cisco SD-WAN Manager, Chrome V8, and Arista EOS to its KEV catalog.
## Key Points
- CISA는 Cisco SD-WAN Manager, Chrome V8 및 Arista EOS에서 적극적으로 악용되는 결함 3개를 KEV 카탈로그에 추가했습니다.
- 미국
- CISA(사이버보안 및 인프라 보안국)는 활성 악용에 대한 보고에 따라 화요일에 알려진 악용 취약점(KEV) 카탈로그에 세 가지 새로운 취약점을 추가했습니다.
## Excerpt
미국 사이버보안 및 인프라 보안국(CISA)은 활성 악용이 보고된 후 화요일에 알려진 악용 취약점(KEV) 카탈로그에 세 가지 새로운 취약점을 추가했습니다. 취약점 목록은 다음과 같습니다. "VXLAN(Virtual Extensible LAN), 디캡 그룹 또는 GRE(Generic Routing Encapsulation) 터널 인터페이스와 같은 터널 캡슐화 해제 구성이 존재하는 Arista EOS를 실행하는 영향을 받는 플랫폼에서 스위치는 구성된 캡슐화 해제 IP와 일치하는 대상 IP를 사용하여 예상치 못한 다른 터널링 패킷을 잘못 캡슐화 해제하고 전달합니다."라고 Arista는 말했습니다. "이는 스위치가 터널 프로토콜 유형을 확인하지 않기 때문에 발생하며 잠재적으로 구성되지 않은 터널 트래픽이 예기치 않게 처리될 수 있습니다." 보안 결함은 주로 7020R, 7280R/R2, 7500R/R2 시리즈 제품에 영향을 미칩니다. 그러나 성공적으로 악용하려면 장치를 VXLAN VTEP, GRE 터널 끝점 또는 IP decap-group과 같은 캡슐화 해제 IP가 있는 터널 끝점으로 구성해야 합니다.