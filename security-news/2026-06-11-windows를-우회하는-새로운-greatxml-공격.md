# Windows를 우회하는 새로운 Greatxml 공격
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/new-greatxml-exploit-bypasses-windows.html
- Published At: unknown
- Collected At: 2026-06-11T23:50:45.372Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Windows-Greatxml-37cfc93aec578136a528c4d46e8b27ed
- Original Title: New Greatxml Exploit Bypasses Windows
## Summary
GreatXML은 Defender 오프라인 검사가 사용된 Windows 시스템에서 BitLocker를 우회하여 암호화된 드라이브 데이터를 노출할 수 있습니다. 보안 연구원인 Chaotic Eclipse(일명 Nightmare-Eclipse 및 MSNightmare)는 Microsoft Defender에 대한 익스플로잇을 발표한 지 하루 만에 GreatXML이라는 새로운 Windows BitLocker 우회를 출시했습니다. 연구원은 블로거에 올린 글에서 "이것은 우연한 발견이었다. 이를 찾는 데 총 4시간이 걸렸다"고 말했다. "Windows Defender 오프라인 검사를 사용하려고 시도한 경우 자동으로 BitLocker 우회에 취약해집니다. 오프라인 검사 기능을 사용하지 않고도 여전히 버그를 유발할 수 있는지 확신할 수 없습니다. 왜냐하면 확실히 그렇게 할 수 있기 때문입니다." 모든 단계를 공동으로 따르면…

## Original Description

GreatXML can bypass BitLocker on Windows systems where Defender Offline Scan was used, exposing encrypted drive data.
## Key Points
- GreatXML은 Defender 오프라인 검사가 사용된 Windows 시스템에서 BitLocker를 우회하여 암호화된 드라이브 데이터를 노출할 수 있습니다.
- 보안 연구원인 Chaotic Eclipse(일명 Nightmare-Eclipse 및 MSNightmare)는 Microsoft Defender에 대한 익스플로잇을 발표한 지 하루 만에 GreatXML이라는 새로운 Windows BitLocker 우회를 출시했습니다.
- 연구원은 블로거에 올린 글에서 "이것은 우연한 발견이었다. 이를 찾는 데 총 4시간이 걸렸다"고 말했다.
## Excerpt
보안 연구원인 Chaotic Eclipse(일명 Nightmare-Eclipse 및 MSNightmare)는 Microsoft Defender에 대한 익스플로잇을 발표한 지 하루 만에 GreatXML이라는 새로운 Windows BitLocker 우회를 출시했습니다. 연구원은 블로거에 올린 글에서 "이것은 우연한 발견이었다. 이를 찾는 데 총 4시간이 걸렸다"고 말했다. "Windows Defender 오프라인 검사를 사용하려고 시도한 경우 자동으로 BitLocker 우회에 취약해집니다. 오프라인 검사 기능을 사용하지 않고도 여전히 버그를 유발할 수 있는지 확신할 수 없습니다. 왜냐하면 확실히 그렇게 할 수 있기 때문입니다." 모든 단계를 올바르게 수행하면 결과적으로 BitLocker 볼륨에 대한 무제한 액세스가 가능한 셸이 생성됩니다. "Defender 오프라인 검사가 시작되지 않은 경우 로그인하여 직접 시작하거나 오프라인 검사 상태에서 WinRE로 부팅하는 방법을 찾아내고(로그인하지 않고도 그렇게 하는 것이 가능하다고 생각합니다) 위의 단계를 따라야 합니다."라고 Chaotic Eclipse는 말했습니다. GreatXML의 출시는 시스템에 대한 LPE(로컬 권한 상승)를 용이하게 하여 공격자가 임의 코드를 실행하거나 무단 작업을 수행할 수 있는 능력을 부여하는 Microsoft Defender의 제로데이 결함인 RoguePlanet 이후 얼마 지나지 않아 출시되었습니다.