# Laravel Lang Php 패키지가 손상되었습니다.
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/05/laravel-lang-php-packages-compromised.html
- Published At: unknown
- Collected At: 2026-05-25T15:39:26.180Z
- Notion Page: https://www.notion.so/The-Hacker-News-Laravel-Lang-Php-36bfc93aec5781549209c0cfaca2a9c1
- Original Title: Laravel Lang Php Packages Compromised
## Summary
Laravel-Lang은 2026년 5월 22~23일에 700개 이상의 버전에 태그를 지정하여 자격 증명을 유출하는 PHP 스틸러를 유발했습니다. 사이버 보안 연구원들은 포괄적인 자격 증명 도용 프레임워크를 제공하기 위해 Laravel-Lang에 속한 여러 PHP 패키지를 표적으로 삼는 새로운 소프트웨어 공급망 공격 캠페인을 발견했습니다. 소켓은 "새로 게시된 태그의 시기와 패턴은 단일 악성 패키지 버전이 아니라 Laravel Lang 조직의 릴리스 프로세스에 대한 광범위한 손상을 가리킨다"고 말했습니다. "태그는 2026년 5월 22일과 5월 23일에 빠르게 연속해서 게시되었으며, 많은 버전이 단 몇 초 간격으로 표시되었습니다." 이 패키지와 관련된 700개 이상의 버전…

## Original Description

Laravel-Lang compromise tagged 700+ versions on May 22–23, 2026, triggering PHP stealers that exfiltrate credentials.
## Key Points
- Laravel-Lang은 2026년 5월 22~23일에 700개 이상의 버전에 태그를 지정하여 자격 증명을 유출하는 PHP 스틸러를 유발했습니다.
- 사이버 보안 연구원들은 포괄적인 자격 증명 도용 프레임워크를 제공하기 위해 Laravel-Lang에 속한 여러 PHP 패키지를 표적으로 삼는 새로운 소프트웨어 공급망 공격 캠페인을 발견했습니다.
- 소켓은 "새로 게시된 태그의 시기와 패턴은 단일 악성 패키지 버전이 아니라 Laravel Lang 조직의 릴리스 프로세스에 대한 광범위한 손상을 가리킨다"고 말했습니다.
## Excerpt
사이버 보안 연구원들은 포괄적인 자격 증명 도용 프레임워크를 제공하기 위해 Laravel-Lang에 속한 여러 PHP 패키지를 표적으로 삼는 새로운 소프트웨어 공급망 공격 캠페인을 발견했습니다. 소켓은 "새로 게시된 태그의 시기와 패턴은 단일 악성 패키지 버전이 아니라 Laravel Lang 조직의 릴리스 프로세스에 대한 광범위한 손상을 가리킨다"고 말했습니다. "태그는 2026년 5월 22일과 5월 23일에 빠르게 연속해서 게시되었으며, 많은 버전이 단 몇 초 간격으로 표시되었습니다." 이러한 패키지와 관련된 700개 이상의 버전이 식별되었으며 이는 자동화된 대량 태그 지정 또는 재출판을 나타냅니다. 공격자가 조직 수준 자격 증명, 저장소 자동화 또는 릴리스 인프라에 대한 액세스 권한을 획득한 것으로 의심됩니다. 이 공격의 차별점은 실제 프로젝트의 소스 코드가 악성코드를 포함하도록 변경되지 않았다는 점입니다. 대신 공격자는 새로운 악성 커밋을 가리키도록 각 저장소의 모든 기존 git 태그를 다시 작성했습니다. 핵심 악성 기능은 버전 태그에 포함된 "src/helpers.php"라는 파일에 있습니다. 이는 주로 감염된 호스트의 지문을 채취하고 외부 서버("flipboxstudio[.]info")에 연결하여 Windows, Linux 및 macOS에서 실행되는 PHP 기반 크로스 플랫폼 페이로드를 검색하도록 설계되었습니다.