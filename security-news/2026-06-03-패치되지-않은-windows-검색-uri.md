# 패치되지 않은 Windows 검색 Uri
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/unpatched-windows-search-uri.html
- Published At: unknown
- Collected At: 2026-06-03T12:31:55.800Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Windows-Uri-374fc93aec57816aaa01c8f6f672a6e6
- Original Title: Unpatched Windows Search Uri
## Summary
패치되지 않은 Windows 검색: URI 결함으로 인해 SMB 요청을 통해 NTLMv2 해시가 유출됩니다. 2026년 4월 공개되어 릴레이 공격이 가능해졌습니다. 사이버 보안 연구원들은 사용자의 NTLMv2 해시를 공격자에게 공개하는 데 악용될 수 있는 패치되지 않은 문제에 대한 세부 정보를 공개했습니다. Windows 캡처 도구의 ms-screensketch: URI 처리기에 영향을 준 CVE-2026-33829의 경우와 마찬가지로 Huntress에 따라 새로 플래그가 지정된 문제는 search: URI 처리기에 있습니다. CVE-2026-33829는 승인되지 않은 행위자에게 중요한 정보를 노출할 수 있는 스푸핑 취약점을 나타냅니다. 이는 2026년 4월 마이크로소프트에 의해 패치되었습니다. "공격자는 사용자가 웹 브라우저에서 특수 제작된 링크를 클릭하도록 유도할 수 있습니다…

## Original Description

Unpatched Windows search: URI flaw leaks NTLMv2 hashes via SMB requests; disclosed April 2026, enabling relay attacks.
## Key Points
- 패치되지 않은 Windows 검색: URI 결함으로 인해 SMB 요청을 통해 NTLMv2 해시가 유출됩니다. 2026년 4월 공개되어 릴레이 공격이 가능해졌습니다.
- 사이버 보안 연구원들은 사용자의 NTLMv2 해시를 공격자에게 공개하는 데 악용될 수 있는 패치되지 않은 문제에 대한 세부 정보를 공개했습니다.
- Windows 캡처 도구의 ms-screensketch: URI 처리기에 영향을 준 CVE-2026-33829의 경우와 마찬가지로 Huntress에 따라 새로 플래그가 지정된 문제는 search: URI 처리기에 있습니다.
## Excerpt
사이버 보안 연구원들은 사용자의 NTLMv2 해시를 공격자에게 공개하는 데 악용될 수 있는 패치되지 않은 문제에 대한 세부 정보를 공개했습니다. Windows 캡처 도구의 ms-screensketch: URI 처리기에 영향을 준 CVE-2026-33829의 경우와 마찬가지로 Huntress에 따라 새로 플래그가 지정된 문제는 search: URI 처리기에 있습니다. CVE-2026-33829는 승인되지 않은 행위자에게 중요한 정보를 노출할 수 있는 스푸핑 취약점을 나타냅니다. 이는 2026년 4월 마이크로소프트에 의해 패치되었습니다. 마이크로소프트는 당시 권고에서 "공격자는 웹 페이지나 이메일 메시지에 삽입하여 사용자가 웹 브라우저나 기타 URL 소스에서 특수 제작된 링크를 클릭하도록 유도할 수 있습니다"라고 밝혔습니다. "사용자가 링크 실행을 승인하면 조작된 URL은 공격자가 선택한 SMB 서버에 컴퓨터를 연결하도록 유도할 수 있으며, 이로 인해 사용자의 NTLMv2 해시가 공격자에게 공개되고 공격자는 이를 사용하여 사용자를 인증할 수 있습니다."