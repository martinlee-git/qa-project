# 악성 Npm 패키지가 Postcss로 가장함
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/malicious-npm-packages-pose-as-postcss.html
- Published At: unknown
- Collected At: 2026-06-23T11:05:36.420Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Npm-Postcss-388fc93aec57817a9e9cf7d17da97d29
- Original Title: Malicious Npm Packages Pose As Postcss
## Summary
JFrog는 Windows RAT를 배포하여 Chrome 자격 증명을 도용하고, 명령을 실행하고, 파일을 전송하는 악성 npm 패키지를 발견했습니다. 사이버 보안 연구원들이 Windows 기반 원격 액세스 트로이 목마(RAT)를 전달하도록 설계된 악성 npm 패키지 세트를 발견했습니다. 확인된 패키지 목록은 다음과 같습니다. 모든 패키지는 "abdrizak"이라는 npm 사용자에 의해 지난 한 달 동안 게시되었으며 이 글을 쓰는 현재 npm에서 계속 다운로드할 수 있습니다. JFrog는 분석에서 "Aes-decode-runner-pro와 postcss-minify-selector-parser는 둘 다 계층화된 AES/custom-codec 패키지로 나타나며 합법적인 postcss-selector-parser에 의존합니다"라고 말했습니다. "Postcss-minify-selector가 제공됩니다…

## Original Description

JFrog found malicious npm packages that deploy a Windows RAT to steal Chrome credentials, run commands, and transfer files.
## Key Points
- JFrog는 Windows RAT를 배포하여 Chrome 자격 증명을 도용하고, 명령을 실행하고, 파일을 전송하는 악성 npm 패키지를 발견했습니다.
- 사이버 보안 연구원들이 Windows 기반 원격 액세스 트로이 목마(RAT)를 전달하도록 설계된 악성 npm 패키지 세트를 발견했습니다.
- 확인된 패키지 목록은 다음과 같습니다. 모든 패키지는 "abdrizak"이라는 npm 사용자에 의해 지난 한 달 동안 게시되었으며 이 글을 쓰는 현재 npm에서 계속 다운로드할 수 있습니다.
## Excerpt
사이버 보안 연구원들이 Windows 기반 원격 액세스 트로이 목마(RAT)를 전달하도록 설계된 악성 npm 패키지 세트를 발견했습니다. 확인된 패키지 목록은 다음과 같습니다. 모든 패키지는 "abdrizak"이라는 npm 사용자에 의해 지난 한 달 동안 게시되었으며 이 글을 쓰는 현재 npm에서 계속 다운로드할 수 있습니다. JFrog는 분석에서 "Aes-decode-runner-pro와 postcss-minify-selector-parser는 둘 다 계층화된 AES/custom-codec 패키지로 나타나며 합법적인 postcss-selector-parser에 의존합니다"라고 말했습니다. "Postcss-minify-selector는 PostCSS 선택기 축소기로 표시되며 postcss-minify-selector-parser에 의존합니다." "postcss-minify-selector-parser"의 이름은 주간 다운로드 수가 1억 2,700만 건 이상인 널리 사용되는 npm 라이브러리인 "postcss-selector-parser"를 참조한 것입니다. 다운로드한 패키지에 관계없이 공격 체인은 동일한 Windows 악성 코드의 배포로 이어집니다.