# Pcpjack, Google Cloud 230AWS 탈취
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/pcpjack-hijacks-230-aws-google-cloud.html
- Published At: unknown
- Collected At: 2026-06-05T09:03:55.137Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Pcpjack-Google-Cloud-230AWS-376fc93aec57810ab69bd5d702d87fe2
- Original Title: Pcpjack Hijacks 230 Aws Google Cloud
## Summary
PCPJack은 하이재킹된 클라우드 서버에서 230노드 SMTP 릴레이를 구축하여 확장 가능한 남용을 위해 5분마다 확인된 프록시를 동기화했습니다. PCPJack으로 알려진 위협 행위자는 AWS(Amazon Web Services), Google Cloud 및 Microsoft Azure와 관련된 클라우드 서버를 하이재킹하여 은밀한 SMTP 이메일 릴레이 네트워크를 만들었습니다. Hunt.io는 성명을 통해 "미국, 유럽, 아시아 전역의 손상된 비즈니스 서버는 조용히 SMTP 프록시로 변환되고 메일 릴레이 기능이 확인되었으며 5분마다 다운스트림 소비자와 동기화되었습니다"라고 밝혔습니다. "우리가 발견했을 당시 인프라는 여전히 실행 중이었습니다." 위협 정보 회사는 소스 코드, 컴파일된 바이너리, 배포 상태 로그 등을 발견했다고 밝혔습니다.

## Original Description

PCPJack built a 230-node SMTP relay from hijacked cloud servers, syncing verified proxies every five minutes for scalable abuse.
## Key Points
- PCPJack은 하이재킹된 클라우드 서버에서 230노드 SMTP 릴레이를 구축하여 확장 가능한 남용을 위해 5분마다 확인된 프록시를 동기화했습니다.
- PCPJack으로 알려진 위협 행위자는 AWS(Amazon Web Services), Google Cloud 및 Microsoft Azure와 관련된 클라우드 서버를 하이재킹하여 은밀한 SMTP 이메일 릴레이 네트워크를 만들었습니다.
- Hunt.io는 성명을 통해 "미국, 유럽, 아시아 전역의 손상된 비즈니스 서버는 조용히 SMTP 프록시로 변환되고 메일 릴레이 기능이 확인되었으며 5분마다 다운스트림 소비자와 동기화되었습니다"라고 밝혔습니다.
## Excerpt
PCPJack으로 알려진 위협 행위자는 AWS(Amazon Web Services), Google Cloud 및 Microsoft Azure와 관련된 클라우드 서버를 하이재킹하여 은밀한 SMTP 이메일 릴레이 네트워크를 만들었습니다. Hunt.io는 성명을 통해 "미국, 유럽, 아시아 전역의 손상된 비즈니스 서버는 조용히 SMTP 프록시로 변환되고 메일 릴레이 기능이 확인되었으며 5분마다 다운스트림 소비자와 동기화되었습니다"라고 밝혔습니다. "우리가 발견했을 당시 인프라는 여전히 실행 중이었습니다." 위협 인텔리전스 회사는 작업 배후의 위협 행위자가 인증 없이 명령 및 제어(C2) 서버("213.136.80[.]73")에 두 개의 공개 디렉터리를 남겨둔 후 소스 코드, 컴파일된 바이너리, 배포 상태 로그, 인터넷 스캐너, 악용 도구 및 라이브 Sliver 구성을 발견했다고 밝혔습니다. PCPJack은 최근 몇 달 동안 소프트웨어 공급망 공격으로 주목을 받은 또 다른 악명 높은 해킹 그룹인 TeamPCP와 관련된 프로세스나 아티팩트를 종료하고 제거하는 조치를 취하는 동시에 특히 클라우드 서비스를 표적으로 삼는 자격 증명 도용 프레임워크를 식별한 후 SentinelOne에 의해 2026년 4월에 처음 발견되었습니다. AMD64, ARM64 및 x86과 같은 대부분의 Linux CPU 아키텍처를 위한 Chisel 터널링 및 프록시 바이너리와 함께 오픈 디렉토리 Sliver 통합 SMTP 프록시 배포 툴킷 중 하나에 준비되어 있습니다. 피해자 측에서는 바이너리가 숨겨진 점 접두사 파일로 삭제되고 "/var/tmp/.xs"에 유지됩니다.