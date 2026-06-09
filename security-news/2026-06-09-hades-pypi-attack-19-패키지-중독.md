# Hades Pypi Attack 19 패키지 중독
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/hades-pypi-attack-19-packages-poisoned.html
- Published At: unknown
- Collected At: 2026-06-09T11:11:47.835Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Hades-Pypi-Attack-19-37afc93aec57810e9a38fbb9fb447002
- Original Title: Hades Pypi Attack 19 Packages Poisoned
## Summary
Mini Shai-Hulud/Miasma 공급망 캠페인의 새로운 PyPI 지점인 Hades는 19개 패키지에 걸쳐 37개의 악성 바퀴를 공격했습니다. Miasma 공급망 캠페인은 Hades라는 새로운 공격 물결을 촉발시켰습니다. 이번에는 Python Package Index(PyPI) 레지스트리의 19개 패키지에 걸쳐 37개의 악성 휠 아티팩트가 관련되어 있습니다. Mini Shai-Hulud 스타일 공격은 특정 생태계를 표적으로 삼기 위해 계속해서 정교해지고 쪼개지고 있습니다. 소켓은 새로운 분석에서 "손상된 릴리스는 Python 시작 중에 자동으로 실행을 시도하고 Bun JavaScript 런타임을 다운로드하며 _index.js라는 난독화된 JavaScript 페이로드를 실행하려고 시도하는 *-setup.pth 파일을 제공했습니다."라고 밝혔습니다. 식별된 패키지 목록은 다음과 같습니다.

## Original Description

Hades, a new PyPI branch of the Mini Shai-Hulud/Miasma supply chain campaign, hit 37 malicious wheels across 19 packages.
## Key Points
- Mini Shai-Hulud/Miasma 공급망 캠페인의 새로운 PyPI 지점인 Hades는 19개 패키지에 걸쳐 37개의 악성 바퀴를 공격했습니다.
- Miasma 공급망 캠페인은 Hades라는 새로운 공격 물결을 촉발시켰습니다. 이번에는 Python Package Index(PyPI) 레지스트리의 19개 패키지에 걸쳐 37개의 악성 휠 아티팩트가 관련되어 있습니다. Mini Shai-Hulud 스타일 공격은 특정 생태계를 표적으로 삼기 위해 계속해서 정교해지고 쪼개지고 있습니다.
- 소켓은 새로운 분석에서 "손상된 릴리스는 Python 시작 중에 자동으로 실행을 시도하고 Bun JavaScript 런타임을 다운로드하며 _index.js라는 난독화된 JavaScript 페이로드를 실행하려고 시도하는 *-setup.pth 파일을 제공했습니다."라고 밝혔습니다.
## Excerpt
Miasma 공급망 캠페인은 Hades라는 새로운 공격 물결을 촉발시켰습니다. 이번에는 Python Package Index(PyPI) 레지스트리의 19개 패키지에 걸쳐 37개의 악성 휠 아티팩트가 관련되어 있습니다. Mini Shai-Hulud 스타일 공격은 특정 생태계를 표적으로 삼기 위해 계속해서 정교해지고 쪼개지고 있습니다. 소켓은 새로운 분석에서 "손상된 릴리스는 Python 시작 중에 자동으로 실행을 시도하고 Bun JavaScript 런타임을 다운로드하며 _index.js라는 난독화된 JavaScript 페이로드를 실행하려고 시도하는 *-setup.pth 파일을 제공했습니다."라고 밝혔습니다. 식별된 패키지 목록은 다음과 같습니다. 이전 Shai-Hulud 및 Miasma 캠페인과 마찬가지로 악성 페이로드는 Bun JavaScript 런타임을 다운로드 및 설치한 다음 개발자 시스템에서 광범위한 데이터를 수집할 수 있는 매우 난독화된 JavaScript 스틸러를 실행하는 데 사용됩니다. 여기에는 Docker 구성, Vault 토큰, SSH 키, 셸 기록, .env 파일, .npmrc 파일, .pypirc 파일, Claude/MCP 구성 및 기타 로컬 또는 러너 액세스 가능 자격 증명과 함께 GitHub, npm, PyPI, RubyGems, JFrog, CircleCI, Anthropic, AWS, GCP, Azure 및 Kubernetes와 관련된 비밀이 포함됩니다.