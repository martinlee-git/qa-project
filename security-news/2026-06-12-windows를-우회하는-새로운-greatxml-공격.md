# Windows를 우회하는 새로운 Greatxml 공격
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/new-greatxml-exploit-bypasses-windows.html
- Published At: unknown
- Collected At: 2026-06-12T05:53:47.717Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Windows-Greatxml-37cfc93aec578136a528c4d46e8b27ed
- Original Title: New Greatxml Exploit Bypasses Windows
## Summary
GreatXML은 Defender 오프라인 검사가 사용된 Windows 시스템에서 BitLocker를 우회하여 암호화된 드라이브 데이터를 노출할 수 있습니다. 보안 연구원인 Chaotic Eclipse(일명 Nightmare-Eclipse 및 MSNightmare)는 Microsoft Defender에 대한 익스플로잇을 발표한 지 하루 만에 GreatXML이라는 새로운 Windows BitLocker 우회를 출시했습니다. 연구원은 블로거에 올린 글에서 "이것은 우연한 발견이었다. 이를 찾는 데 총 4시간이 걸렸다"고 말했다. "Windows Defender 오프라인 검사를 사용하려고 시도한 경우 자동으로 BitLocker 우회에 취약해집니다. 오프라인 검사 기능을 사용하지 않고도 여전히 버그를 유발할 수 있는지 확신할 수 없습니다. 왜냐하면 확실히 그렇게 할 수 있기 때문입니다." 모든 단계를 따르면…

## Original Description

GreatXML can bypass BitLocker on Windows systems where Defender Offline Scan was used, exposing encrypted drive data.
## Key Points
- GreatXML은 Defender 오프라인 검사가 사용된 Windows 시스템에서 BitLocker를 우회하여 암호화된 드라이브 데이터를 노출할 수 있습니다.
- 보안 연구원인 Chaotic Eclipse(일명 Nightmare-Eclipse 및 MSNightmare)는 Microsoft Defender에 대한 익스플로잇을 발표한 지 하루 만에 GreatXML이라는 새로운 Windows BitLocker 우회를 출시했습니다.
- 연구원은 블로거에 올린 글에서 "이것은 우연한 발견이었다. 이를 찾는 데 총 4시간이 걸렸다"고 말했다.
## Excerpt
보안 연구원인 Chaotic Eclipse(일명 Nightmare-Eclipse 및 MSNightmare)는 Microsoft Defender에 대한 익스플로잇을 발표한 지 하루 만에 GreatXML이라는 새로운 Windows BitLocker 우회를 출시했습니다. 연구원은 블로거에 올린 글에서 "이것은 우연한 발견이었다. 이를 찾는 데 총 4시간이 걸렸다"고 말했다. "Windows Defender 오프라인 검사를 사용하려고 시도한 경우 자동으로 BitLocker 우회에 취약해집니다. 오프라인 검사 기능을 사용하지 않고도 여전히 버그를 유발할 수 있는지 확신할 수 없습니다. 왜냐하면 확실히 그렇게 할 수 있기 때문입니다." 모든 단계를 올바르게 수행하면 결과적으로 BitLocker 볼륨에 대한 무제한 액세스가 가능한 셸이 생성됩니다. "Defender 오프라인 검사가 시작되지 않은 경우 로그인하여 직접 시작하거나 오프라인 검사 상태에서 WinRE로 부팅하는 방법을 찾아내고(로그인하지 않고도 그렇게 하는 것이 가능하다고 생각합니다) 위의 단계를 따라야 합니다."라고 Chaotic Eclipse는 말했습니다. Mastodon에 대한 게시물에서 보안 연구원인 Will Dormann은 GreatXML을 "결함이 있는" 것으로 재생산하는 단계에 대해 의견을 밝혔으며, Microsoft Defender 오프라인 검사를 실행하려면 사용자가 Windows에 로그인하고 관리자 자격 증명을 가지고 있어야 하기 때문에 어쨌든 BitLocker를 끄는 것이 쉽지 않습니다.