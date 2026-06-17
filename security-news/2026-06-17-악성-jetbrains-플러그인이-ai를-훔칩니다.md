# 악성 Jetbrains 플러그인이 Ai를 훔칩니다.
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/malicious-jetbrains-plugins-steal-ai.html
- Published At: unknown
- Collected At: 2026-06-17T15:23:42.451Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Jetbrains-Ai-382fc93aec578108b179d62353320e8b
- Original Title: Malicious Jetbrains Plugins Steal Ai
## Summary
연구원들은 OpenAI, DeepSeek 및 SiliconFlow API 키를 유출하는 AI 코딩 도구로 위장한 악성 JetBrains 플러그인 15개를 발견했습니다. 사이버 보안 연구원들이 JetBrains Marketplace에서 인공 지능(AI) 공급자 키를 유출할 수 있는 악성 플러그인을 15개 이상 게시한 "조정된 악성 코드 캠페인"을 표시했습니다. Aikido Security 연구원 Ilyas Makari는 "모든 플러그인은 DeepSeek 및 기타 대규모 언어 모델을 기반으로 구축된 AI 코딩 도우미 역할을 하며 채팅, 커밋 메시지, 코드 검토, 버그 찾기 및 단위 테스트를 제공합니다."라고 말했습니다. "광고한 대로 정확하게 작동합니다. 하지만 입력한 AI 제공업체 API 키는 다음에 의해 제어되는 서버로 유출됩니다.

## Original Description

Researchers found 15 malicious JetBrains plugins posing as AI coding tools that exfiltrate OpenAI, DeepSeek, and SiliconFlow API keys.
## Key Points
- 연구원들은 OpenAI, DeepSeek 및 SiliconFlow API 키를 유출하는 AI 코딩 도구로 위장한 악성 JetBrains 플러그인 15개를 발견했습니다.
- 사이버 보안 연구원들이 JetBrains Marketplace에서 인공 지능(AI) 공급자 키를 유출할 수 있는 악성 플러그인을 15개 이상 게시한 "조정된 악성 코드 캠페인"을 표시했습니다.
- Aikido Security 연구원 Ilyas Makari는 "모든 플러그인은 DeepSeek 및 기타 대규모 언어 모델을 기반으로 구축된 AI 코딩 도우미 역할을 하며 채팅, 커밋 메시지, 코드 검토, 버그 찾기 및 단위 테스트를 제공합니다."라고 말했습니다.
## Excerpt
사이버 보안 연구원들이 JetBrains Marketplace에서 인공 지능(AI) 공급자 키를 유출할 수 있는 악성 플러그인을 15개 이상 게시한 "조정된 악성 코드 캠페인"을 표시했습니다. Aikido Security 연구원 Ilyas Makari는 "모든 플러그인은 DeepSeek 및 기타 대규모 언어 모델을 기반으로 구축된 AI 코딩 도우미 역할을 하며 채팅, 커밋 메시지, 코드 검토, 버그 찾기 및 단위 테스트를 제공합니다."라고 말했습니다. "광고한 대로 정확하게 작동합니다. 그러나 입력한 AI 공급자 API 키는 공격자가 제어하는 ​​서버로 유출됩니다." 이 활동은 2025년 10월 말부터 진행된 것으로 알려졌으며 최근에는 2026년 6월 10일에 새로운 플러그인이 출시되었습니다. 두 플러그인인 CodeGPT AI Assistant와 DeepSeek AI Assist는 각각 25,000회 이상의 다운로드를 기록했지만, 그 수가 진짜인지, 아니면 인기를 위조하기 위해 부풀려졌는지는 확실하지 않습니다. Aikido Security는 15개 플러그인 모두 유사한 코드베이스를 공유하므로 사용자가 약속된 기능을 수행하려면 설정 패널을 열고 OpenAI, SiliconFlow 또는 DeepSeek와 같은 AI에 대한 API 키를 입력해야 한다고 말했습니다. 플러그인이 의도한 대로 작동하는 동안 일반 텍스트 형식의 HTTP 요청에 대한 공격자의 제어 하에 제공된 API 키를 원격 서버("39.107.60[.]51")에 은밀하게 사이펀하는 기능을 몰래 삽입하는 것으로 밝혀졌습니다.