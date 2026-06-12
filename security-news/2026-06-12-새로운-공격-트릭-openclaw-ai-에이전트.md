# 새로운 공격 트릭 Openclaw Ai 에이전트
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/new-attacks-trick-openclaw-ai-agent.html
- Published At: unknown
- Collected At: 2026-06-12T00:50:47.243Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Openclaw-Ai-37cfc93aec5781b39aeecc34a6dae436
- Original Title: New Attacks Trick Openclaw Ai Agent
## Summary
OpenClaw 입력 결함으로 인해 숨겨진 연락처와 피싱 이메일이 코드 실행 및 데이터 유출을 유발하여 에이전트 신뢰 위험을 노출시킬 수 있습니다. 두 보안 팀은 이번 주에 발표된 별도의 연구에서 인기 있는 자체 호스팅 AI 에이전트인 OpenClaw가 공격자가 제어하는 ​​코드를 실행하거나 평범해 보이는 입력을 통해 민감한 데이터를 넘겨주도록 유도할 수 있음을 보여주었습니다. Imperva는 피해자가 보지 못한 채 에이전트가 실행한 공유 연락처, vCard, 위치 핀 내부에 지침을 묻어두었습니다. Varonis는 플랫폼에 테스트 에이전트를 구축하고 합성 비즈니스 데이터로 가득 찬 메일박스를 제공한 후 모의 AWS 키와 가짜 고객 내보내기를 외부로 전달하라는 일반 이메일 하나를 지켜보았습니다.

## Original Description

OpenClaw input flaws let hidden contacts and phishing emails trigger code execution and data leaks, exposing agent trust risks.
## Key Points
- OpenClaw 입력 결함으로 인해 숨겨진 연락처와 피싱 이메일이 코드 실행 및 데이터 유출을 유발하여 에이전트 신뢰 위험을 노출시킬 수 있습니다.
- 두 보안 팀은 이번 주에 발표된 별도의 연구에서 인기 있는 자체 호스팅 AI 에이전트인 OpenClaw가 공격자가 제어하는 ​​코드를 실행하거나 평범해 보이는 입력을 통해 민감한 데이터를 넘겨주도록 유도할 수 있음을 보여주었습니다.
- Imperva는 피해자가 보지 못한 채 에이전트가 실행한 공유 연락처, vCard, 위치 핀 내부에 지침을 묻어두었습니다.
## Excerpt
두 보안 팀은 이번 주에 발표된 별도의 연구에서 인기 있는 자체 호스팅 AI 에이전트인 OpenClaw가 공격자가 제어하는 ​​코드를 실행하거나 평범해 보이는 입력을 통해 민감한 데이터를 넘겨주도록 유도할 수 있음을 보여주었습니다. Imperva는 피해자가 보지 못한 채 에이전트가 실행한 공유 연락처, vCard, 위치 핀 내부에 지침을 묻어두었습니다. Varonis는 플랫폼에 테스트 에이전트를 구축하고 합성 비즈니스 데이터로 가득 찬 메일함을 제공한 후 모의 AWS 키와 외부 주소로 가짜 고객 내보내기를 전달하는 일반 이메일 하나를 지켜보았습니다. Imperva가 발견한 취약점은 OpenClaw 2026.4.23에서 패치되었으니, 실행하시면 업데이트해 주세요. Varonis가 발견한 피싱 약점은 패치로 해결되는 것이 아닙니다. 결국 에이전트가 자체적으로 수행할 수 있는 작업이 제한됩니다. 같은 방으로 들어가는 다른 문: 에이전트는 여기에 도달하는 것을 신뢰하고 해당 액세스는 공격자의 것이 됩니다. Imperva 연구원인 Yohann Sillam은 OpenClaw가 메시징 데이터를 그 뒤에 있는 모델에 전달하는 방법을 살펴보았습니다. 문제는 배관에 있습니다.