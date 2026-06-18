# 주니어 해커는 Tailscale을 사용했으며
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/junior-hacker-used-tailscale-and.html
- Published At: unknown
- Collected At: 2026-06-18T11:38:42.321Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Tailscale-382fc93aec5781caa804c08ecde93327
- Original Title: Junior Hacker Used Tailscale And
## Summary
Cato Networks는 33일 간의 침입으로 Havoc C2가 중단된 후 액세스를 유지하기 위해 OpenSSH 및 Tailscale을 사용하여 Poisson을 추적했습니다. 프랑스어를 사용하는 공격자가 프랑스의 소규모 자동차 회사에 침입하여 키로거를 설치하고 은행 및 이메일 자격 증명을 훔쳤습니다. 끝이 가까워질 때까지 평범한 것. 그의 C&C 서버가 꺼지기 전에 그는 피해자의 컴퓨터에 OpenSSH와 Tailscale을 설치하여 C2를 전혀 통과하지 않는 경로를 구축했습니다. 다음 날 Havoc 서버가 오프라인 상태가 되었을 때 그의 액세스는 불가능했습니다. 18일 후 C2가 돌아왔고 그의 에이전트는 스스로 다시 연결되었고 그는 계속했습니다. 카토네트웍스는 전체 작전 명령을 명령으로 포착했고,…

## Original Description

Cato Networks tracked Poisson using OpenSSH and Tailscale to maintain access after Havoc C2 outage in a 33-day intrusion.
## Key Points
- Cato Networks는 33일 간의 침입으로 Havoc C2가 중단된 후 액세스를 유지하기 위해 OpenSSH 및 Tailscale을 사용하여 Poisson을 추적했습니다.
- 프랑스어를 사용하는 공격자가 프랑스의 소규모 자동차 회사에 침입하여 키로거를 설치하고 은행 및 이메일 자격 증명을 훔쳤습니다.
- 끝이 가까워질 때까지 평범한 것.
## Excerpt
프랑스어를 사용하는 공격자가 프랑스의 소규모 자동차 회사에 침입하여 키로거를 설치하고 은행 및 이메일 자격 증명을 훔쳤습니다. 끝이 가까워질 때까지 평범한 것. 그의 C&C 서버가 꺼지기 전에 그는 피해자의 컴퓨터에 OpenSSH와 Tailscale을 설치하여 C2를 전혀 통과하지 않는 경로를 구축했습니다. 다음 날 Havoc 서버가 오프라인 상태가 되었을 때 그의 액세스는 불가능했습니다. 18일 후 C2가 돌아왔고 그의 에이전트는 스스로 다시 연결되었고 그는 계속했습니다. Cato Networks는 운영자가 개방형 스토리지 버킷에 SSH 키와 단계별 플레이북을 남겨둔 후 33일 동안 전체 작업 명령을 명령별로 캡처했습니다. 그 중 339개였습니다. Cato CTRL 연구원인 Vitaly Simonovich가 화요일에 발표한 이 글은 포렌식 남은 부분이 아닌 운영자 키보드의 침입에 대한 보기 드문 견해입니다. 연구원의 교훈은 직설적입니다. 공격자가 이미 별도의 문을 구축한 경우 C2 서버를 오프라인으로 전환하는 것은 치료가 아닙니다.