# Openai Codex 인증 토큰
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/openai-codex-authentication-tokens.html
- Published At: unknown
- Collected At: 2026-06-01T12:59:58.717Z
- Notion Page: https://www.notion.so/The-Hacker-News-Openai-Codex-372fc93aec57811594bffbed3c3afaa7
- Original Title: Openai Codex Authentication Tokens
## Summary
Codex 토큰은 인기 있는 npm 패키지를 통해 유출되어 v0.1.82부터 사용자에게 영향을 미치고 지속적인 계정 액세스를 가능하게 했습니다. 사이버 보안 연구원들이 합법적으로 보이는 원격 웹 UI를 통해 OpenAI Codex를 사용하는 개발자를 표적으로 삼는 새로운 악성 공급망 캠페인의 세부 정보를 공개했습니다. codexui-android라는 이름의 이 도구는 OpenAI Codex용 원격 웹 UI로 GitHub 및 npm에 광고되어 매주 29,000회 이상의 다운로드를 기록하고 있습니다. 패키지는 여전히 저장소에서 다운로드할 수 있습니다. 이 활동이 주목할 만한 점은 개발자를 속이기 위해 타이포스쿼트나 일회용 패키지를 사용하는 전통적인 공격이 아니라는 점입니다. 오히려 악성코드가 내장되어 있는데…

## Original Description

Codex tokens were exfiltrated via a popular npm package, affecting users since v0.1.82 and enabling persistent account access.
## Key Points
- Codex 토큰은 인기 있는 npm 패키지를 통해 유출되어 v0.1.82부터 사용자에게 영향을 미치고 지속적인 계정 액세스를 가능하게 했습니다.
- 사이버 보안 연구원들이 합법적으로 보이는 원격 웹 UI를 통해 OpenAI Codex를 사용하는 개발자를 표적으로 삼는 새로운 악성 공급망 캠페인의 세부 정보를 공개했습니다.
- codexui-android라는 이름의 이 도구는 OpenAI Codex용 원격 웹 UI로 GitHub 및 npm에 광고되어 매주 29,000회 이상의 다운로드를 기록하고 있습니다.
## Excerpt
사이버 보안 연구원들이 합법적으로 보이는 원격 웹 UI를 통해 OpenAI Codex를 사용하는 개발자를 표적으로 삼는 새로운 악성 공급망 캠페인의 세부 정보를 공개했습니다. codexui-android라는 이름의 이 도구는 OpenAI Codex용 원격 웹 UI로 GitHub 및 npm에 광고되어 매주 29,000회 이상의 다운로드를 기록하고 있습니다. 패키지는 여전히 저장소에서 다운로드할 수 있습니다. 이 활동이 주목할 만한 점은 개발자를 속이기 위해 타이포스쿼트나 일회용 패키지를 사용하는 전통적인 공격이 아니라는 점입니다. 오히려 악성 코드는 활발히 개발되고 있는 기능적인 npm 패키지에 내장되어 있습니다. 연결된 GitHub 저장소는 깨끗한 상태로 유지됩니다. Aikido Security 연구원인 Charlie Eriksen은 "지난 달 동안 호출할 때마다 Codex 인증 토큰이 공격자가 제어하는 ​​서버로 조용히 유출되었습니다."라고 말했습니다. 이 사악한 변경 사항은 패키지가 레지스트리에 게시된 지 약 한 달 후에 도입된 것으로 알려져 있으며, 이는 아마도 사용자 신뢰를 구축하고 범위를 확대하려는 노력의 일환일 것입니다. 패키지와 연결된 npm 계정은 "friuns"(일명 Igor Levochkin)입니다.