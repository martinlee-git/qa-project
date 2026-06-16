# 공격자들은 Three Fortinet을 악용했습니다.
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/attackers-exploit-three-fortinet.html
- Published At: unknown
- Collected At: 2026-06-16T16:06:43.785Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Three-Fortinet-381fc93aec5781ba8e33ede88627a35b
- Original Title: Attackers Exploit Three Fortinet
## Summary
공격자들은 지난주 패치된 한 가지를 포함해 Fortinet FortiSandbox의 세 가지 결함을 악용하여 인증 우회 및 명령 실행 위험을 감수하고 있습니다. 위협 정보 회사인 Defused Cyber에 따르면 악의적인 행위자들이 Fortinet FortiSandbox의 여러 보안 취약점을 악용하고 있다고 합니다. X에 공유된 게시물에서 회사는 지난 24시간 동안 CVE-2026-39813, CVE-2026-39808 및 CVE-2026-25089의 악용을 관찰했다고 밝혔습니다. CVE-2026-39813(CVSS 점수: 9.1)은 인증되지 않은 공격자가 특별히 제작된 HTTP 요청을 통해 인증을 우회하도록 허용할 수 있는 FortiSandbox JRPC API의 경로 통과 취약점을 나타냅니다. 두 번째 결함인 CVE-2026-39808(CVSS 점수: 9.1)은 조작 사례입니다.

## Original Description

Attackers are exploiting three Fortinet FortiSandbox flaws, including one patched last week, risking auth bypass and command execution.
## Key Points
- 공격자들은 지난주 패치된 한 가지를 포함해 Fortinet FortiSandbox의 세 가지 결함을 악용하여 인증 우회 및 명령 실행 위험을 감수하고 있습니다.
- 위협 정보 회사인 Defused Cyber에 따르면 악의적인 행위자들이 Fortinet FortiSandbox의 여러 보안 취약점을 악용하고 있다고 합니다.
- X에 공유된 게시물에서 회사는 지난 24시간 동안 CVE-2026-39813, CVE-2026-39808 및 CVE-2026-25089의 악용을 관찰했다고 밝혔습니다.
## Excerpt
위협 정보 회사인 Defused Cyber에 따르면 악의적인 행위자들이 Fortinet FortiSandbox의 여러 보안 취약점을 악용하고 있다고 합니다. X에 공유된 게시물에서 회사는 지난 24시간 동안 CVE-2026-39813, CVE-2026-39808 및 CVE-2026-25089의 악용을 관찰했다고 밝혔습니다. CVE-2026-39813(CVSS 점수: 9.1)은 인증되지 않은 공격자가 특별히 제작된 HTTP 요청을 통해 인증을 우회하도록 허용할 수 있는 FortiSandbox JRPC API의 경로 통과 취약점을 나타냅니다. 두 번째 결함인 CVE-2026-39808(CVSS 점수: 9.1)은 인증되지 않은 공격자가 조작된 HTTP 요청을 통해 인증되지 않은 코드나 명령을 실행할 수 있도록 허용하는 운영 체제 명령 주입 사례입니다. 두 취약점 모두 2026년 4월에 Fortinet에 의해 패치되었습니다. 반면 CVE-2026-25089(CVSS 점수: 9.1)는 지난 주에 수정되었습니다. Fortinet은 이 취약점을 FortiSandbox, FortiSandbox Cloud 및 FortiSandbox PaaS 웹 UI에 영향을 미치는 운영 체제 명령 주입으로 인증되지 않은 공격자가 특별히 조작된 HTTP 요청을 통해 승인되지 않은 명령을 실행할 수 있도록 허용한다고 설명했습니다.