# 인기 있는 WordPress 플러그인 스크립트
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/popular-wordpress-plugin-scripts.html
- Published At: unknown
- Collected At: 2026-06-15T13:47:44.765Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-WordPress-380fc93aec57819ab7ebca3180e3dad2
- Original Title: Popular Wordpress Plugin Scripts
## Summary
세 가지 Awesome Motive 플러그인의 JavaScript가 변조되어 WordPress 사이트가 악성 관리자 계정과 숨겨진 백도어에 노출되었습니다. 공격자는 PushEngage, OptinMonster 및 TrustPulse를 실행하는 WordPress 사이트에서 사용되는 신뢰할 수 있는 JavaScript 파일을 변조하여 해당 파일을 사이트에 침입하는 방법으로 전환했습니다. 파일이 로드되면서 사이트 관리자가 로그인하면 해당 코드는 공격자의 통제하에 있는 관리자 계정을 생성하고 다시 들어올 수 있는 숨겨진 플러그인을 설치했습니다. 일반 방문자는 이를 실행하지 않았습니다. 공격을 받은 모든 사이트는 손상된 것으로 간주되어야 합니다. 세 가지 플러그인 모두 Awesome Motive라는 한 회사에서 운영하고 있는데, 이 회사는 6월 현재 두 개의 대형 플러그인에 대해 언급하지 않았습니다.

## Original Description

Tampered JavaScript in three Awesome Motive plugins exposed WordPress sites to rogue admin accounts and hidden backdoors.
## Key Points
- 세 가지 Awesome Motive 플러그인의 JavaScript가 변조되어 WordPress 사이트가 악성 관리자 계정과 숨겨진 백도어에 노출되었습니다.
- 공격자는 PushEngage, OptinMonster 및 TrustPulse를 실행하는 WordPress 사이트에서 사용되는 신뢰할 수 있는 JavaScript 파일을 변조하여 해당 파일을 사이트에 침입하는 방법으로 전환했습니다.
- 파일이 로드되면서 사이트 관리자가 로그인하면 해당 코드는 공격자의 통제하에 관리자 계정을 생성하고 다시 들어올 수 있는 숨겨진 플러그인을 설치했습니다.
## Excerpt
공격자는 PushEngage, OptinMonster 및 TrustPulse를 실행하는 WordPress 사이트에서 사용되는 신뢰할 수 있는 JavaScript 파일을 변조하여 해당 파일을 사이트에 침입하는 방법으로 전환했습니다. 파일이 로드되면서 사이트 관리자가 로그인하면 해당 코드는 공격자의 통제하에 있는 관리자 계정을 생성하고 다시 들어올 수 있는 숨겨진 플러그인을 설치했습니다. 일반 방문자는 이를 실행하지 않았습니다. 공격을 받은 모든 사이트는 손상된 것으로 간주되어야 합니다. 세 가지 플러그인 모두 Awesome Motive라는 한 회사에서 운영하고 있는데, 이 회사는 6월 15일 현재 두 개의 대형 플러그인에 대해 언급하지 않았습니다. 보안 회사 Sansec은 6월 13일에 더 광범위한 캠페인을 공개했으며, JavaScript에서 세 가지 플러그인 모두에 대해 동일한 악성 코드가 제공되는 것을 발견했습니다. PushEngage는 하루 후 자체 사건 통지를 통해 공격자가 스크립트의 변조된 복사본을 제공했으며 해당 스크립트를 로드하는 사이트가 장악될 수 있음을 확인했습니다.