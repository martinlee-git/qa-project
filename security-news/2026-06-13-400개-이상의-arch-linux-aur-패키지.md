# 400개 이상의 Arch Linux Aur 패키지
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/over-400-arch-linux-aur-packages.html
- Published At: unknown
- Collected At: 2026-06-13T07:11:46.598Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-400-Arch-Linux-Aur-37dfc93aec5781f28e47f591c3f6cbd4
- Original Title: Over 400 Arch Linux Aur Packages
## Summary
공격자들은 루트 시스템에서 선택적으로 eBPF 루트킷을 지원하는 Rust 자격 증명 도용자를 실행하기 위해 400개 이상의 Arch Linux AUR 패키지를 하이재킹했습니다. 공격자들은 이번 주 AUR(Arch User Repository)에서 400개 이상의 패키지를 탈취하고 빌드 스크립트를 다시 작성하여 해당 패키지를 빌드한 모든 시스템에 자격 증명 도용자를 설치했습니다. 이 악성코드는 개발자 비밀을 수집하기 위해 구축된 Rust 바이너리입니다. 루트에 도달하면 eBPF 루트킷을 로드하여 자신을 숨길 수도 있습니다. AUR은 Arch Linux의 커뮤니티 패키지 모음이며 영향을 받지 않은 공식 Arch 리포지토리와 별개입니다. 6월 11일 이후에 AUR 패키지를 설치하거나 업데이트한 경우 현재 영향을 받는 패키지와 비교하여 확인하세요.

## Original Description

Attackers hijacked 400+ Arch Linux AUR packages to run a Rust credential stealer, with optional eBPF rootkit support on root systems.
## Key Points
- 공격자들은 루트 시스템에서 선택적으로 eBPF 루트킷을 지원하는 Rust 자격 증명 도용자를 실행하기 위해 400개 이상의 Arch Linux AUR 패키지를 하이재킹했습니다.
- 공격자들은 이번 주 AUR(Arch User Repository)에서 400개 이상의 패키지를 탈취하고 빌드 스크립트를 다시 작성하여 해당 패키지를 빌드한 모든 시스템에 자격 증명 도용자를 설치했습니다.
- 이 악성코드는 개발자 비밀을 수집하기 위해 구축된 Rust 바이너리입니다.
## Excerpt
공격자들은 이번 주 AUR(Arch User Repository)에서 400개 이상의 패키지를 탈취하고 빌드 스크립트를 다시 작성하여 해당 패키지를 빌드한 모든 시스템에 자격 증명 도용자를 설치했습니다. 이 악성코드는 개발자 비밀을 수집하기 위해 구축된 Rust 바이너리입니다. 루트에 도달하면 eBPF 루트킷을 로드하여 자신을 숨길 수도 있습니다. AUR은 Arch Linux의 커뮤니티 패키지 모음이며 영향을 받지 않은 공식 Arch 리포지토리와 별개입니다. 6월 11일 이후에 AUR 패키지를 설치하거나 업데이트한 경우 호스트를 신뢰하기 전에 현재 영향을 받는 패키지 목록과 비교하여 확인하십시오. 이름 목록은 방대하고 계속 증가하고 있으며 아직 완전하지 않습니다. 이 공격은 소프트웨어 결함이 아닌 신뢰 모델을 따릅니다. 손상된 패키지에는 이름, 기록 및 그에 따른 신뢰가 유지되었습니다. 빌드 지침만 변경되었습니다. 트랩은 레시피에 포함되어 패키지 자체가 사용자가 설치하려는 소프트웨어와 정확히 동일하게 보입니다. 악용도, 제로데이도, 흔적도 없이 Arch의 자체 시스템이 침해되었습니다.