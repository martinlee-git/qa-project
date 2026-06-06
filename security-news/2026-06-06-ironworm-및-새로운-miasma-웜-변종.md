# Ironworm 및 새로운 Miasma 웜 변종
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/ironworm-and-new-miasma-worm-variant.html
- Published At: unknown
- Collected At: 2026-06-06T00:14:53.307Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Ironworm-Miasma-376fc93aec5781008b96cf39ee582586
- Original Title: Ironworm And New Miasma Worm Variant
## Summary
여러 차례의 npm 공급망 공격에서는 Rust 기반 스틸러인 IronWorm과 Miasma 웜 변종을 확산시키기 위해 50개 이상의 중독된 패키지가 사용되었습니다. 다수의 소프트웨어 공급망 공격이 npm 생태계를 강타했으며, 위협 행위자는 50개가 넘는 합법적인 패키지의 악성 버전과 중독된 버전을 모두 사용하여 각각 Rust 기반 정보 도용자와 자체 확산 웜을 배포했습니다. JFrog에 따르면 정보 도둑은 "개발자의 컴퓨터에서 찾을 수 있는 모든 비밀을 긁어내고 eBPF 커널 루트킷 뒤에 숨어 있으며 Tor를 통해 운영자에게 응답합니다." 또한 도둑은 훔친 자격 증명을 전파 메커니즘으로 사용하여 악명 높은 Shai-Hulud 웜과 유사합니다. 새로운 말와…

## Original Description

Multiple npm supply chain attacks used 50+ poisoned packages to spread IronWorm, a Rust-based stealer, and a Miasma worm variant.
## Key Points
- 여러 차례의 npm 공급망 공격에서는 Rust 기반 스틸러인 IronWorm과 Miasma 웜 변종을 확산시키기 위해 50개 이상의 중독된 패키지가 사용되었습니다.
- 다수의 소프트웨어 공급망 공격이 npm 생태계를 강타했으며, 위협 행위자는 50개가 넘는 합법적인 패키지의 악성 버전과 중독된 버전을 모두 사용하여 각각 Rust 기반 정보 도용자와 자체 확산 웜을 배포했습니다.
- JFrog에 따르면 정보 도둑은 "개발자의 컴퓨터에서 찾을 수 있는 모든 비밀을 긁어내고 eBPF 커널 루트킷 뒤에 숨어 있으며 Tor를 통해 운영자에게 응답합니다." 또한 도둑은 훔친 자격 증명을 전파 메커니즘으로 사용하여 악명 높은 Shai-Hulud 웜과 유사합니다.
## Excerpt
다수의 소프트웨어 공급망 공격이 npm 생태계를 강타했으며, 위협 행위자는 50개가 넘는 합법적인 패키지의 악성 버전과 중독된 버전을 모두 사용하여 각각 Rust 기반 정보 도용자와 자체 확산 웜을 배포했습니다. JFrog에 따르면 정보 도둑은 "개발자의 컴퓨터에서 찾을 수 있는 모든 비밀을 긁어내고 eBPF 커널 루트킷 뒤에 숨어 있으며 Tor를 통해 운영자에게 응답합니다." 또한 도둑은 훔친 자격 증명을 전파 메커니즘으로 사용하여 악명 높은 Shai-Hulud 웜과 유사합니다. 소프트웨어 공급망 보안 회사는 새로운 악성 코드의 코드명을 IronWorm으로 지정했습니다. 이 접근 방식은 트로이 목마 패키지 형태로 npm 레지스트리에 자체적으로 게시함으로써 자체 복제 공격을 발생시킵니다. 악성 활동은 사전 설치 후크를 통해 실행되는 Rust ELF 바이너리가 포함된 패키지 버전을 게시하는 것으로 밝혀진 "asteroiddao"라는 손상된 npm 계정으로 추적되었습니다. 이 악성코드는 86개의 환경 변수, OpenAI Codex, Anthropic, Claude, Google Gemini, Cursor, Amazon Web Services(AWS), Docker, Kubernetes 및 npm과 관련된 자격 증명, 볼트 구성 및 Exodus 암호화폐 지갑 파일을 포함할 수 있는 다양한 파일을 표적으로 삼습니다.