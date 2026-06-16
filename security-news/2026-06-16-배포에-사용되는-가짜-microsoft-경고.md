# 배포에 사용되는 가짜 Microsoft 경고
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/fake-microsoft-alerts-used-to-deploy.html
- Published At: unknown
- Collected At: 2026-06-16T11:02:43.691Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Microsoft-381fc93aec5781dfab81f62f73d3ac21
- Original Title: Fake Microsoft Alerts Used To Deploy
## Summary
북한과 연계된 ScarCruft는 가짜 Microsoft 계정 경고와 ZIP 파일을 사용하여 데이터 도난을 위해 구축된 Python RAT인 NarwhalRAT를 전달합니다. ScarCruft(일명 APT37)로 알려진 북한 정부가 후원하는 해킹 그룹이 NarwhalRAT이라는 악성 코드를 전달하기 위해 Microsoft 계정 보안 알림을 사칭하는 스피어 피싱 메시지를 사용하는 것이 관찰되었습니다. 지니언스 보안센터(GSC)는 “공격 이메일에는 MS 계정 보안 경고를 사칭한 메시지가 포함돼 있다”고 밝혔다. "이는 계정 손상 및 OTP 남용 가능성에 대한 우려를 조성하여 수신자가 첨부 파일을 실행하도록 유도하도록 설계되었습니다." "이메일 본문에는 수신자에게 첨부된 권고문을 참조하라고 지시했습니다. H…

## Original Description

North Korea-linked ScarCruft uses fake Microsoft Account alerts and ZIP files to deliver NarwhalRAT, a Python RAT built for data theft.
## Key Points
- 북한과 연계된 ScarCruft는 가짜 Microsoft 계정 경고와 ZIP 파일을 사용하여 데이터 도난을 위해 구축된 Python RAT인 NarwhalRAT를 전달합니다.
- ScarCruft(일명 APT37)로 알려진 북한 정부가 후원하는 해킹 그룹이 NarwhalRAT이라는 악성 코드를 전달하기 위해 Microsoft 계정 보안 알림을 사칭하는 스피어 피싱 메시지를 사용하는 것이 관찰되었습니다.
- 지니언스 보안센터(GSC)는 “공격 이메일에는 MS 계정 보안 경고를 사칭한 메시지가 포함돼 있다”고 밝혔다.
## Excerpt
ScarCruft(일명 APT37)로 알려진 북한 정부가 후원하는 해킹 그룹이 NarwhalRAT이라는 악성 코드를 전달하기 위해 Microsoft 계정 보안 알림을 사칭하는 스피어 피싱 메시지를 사용하는 것이 관찰되었습니다. 지니언스 보안센터(GSC)는 “공격 이메일에는 MS 계정 보안 경고를 사칭한 메시지가 포함돼 있다”고 밝혔다. "이는 계정 손상 및 OTP 남용 가능성에 대한 우려를 조성하여 수신자가 첨부 파일을 실행하도록 유도하도록 설계되었습니다." "이메일 본문은 수신자에게 첨부된 권고문을 참조하라고 지시했습니다. 그러나 실제 첨부파일은 HWP(한글 워드 프로세서) 문서가 아니고 악성 LNK 파일이 포함된 ZIP 아카이브였습니다." 이메일 메시지는 일회용 비밀번호의 반복 생성과 관련된 "비정상적인 활동"을 주장하며 이를 제3자가 대상의 Microsoft 계정을 겨냥한 피싱 시도로 위장하고 비밀번호를 변경하도록 촉구합니다. 피싱 메시지의 최종 목표는 잘못된 긴급감을 유도하고 피해자가 이메일을 합법적인 보안 경고로 해석하도록 속이는 것입니다. LNK 파일이 실행되면 중간 배치 스크립트를 사용하여 NarwhalRAT를 다운로드 및 설치하고 공식 웹 사이트 및 Windows 보안 카탈로그(CAT) 파일에서 합법적인 Python 실행 파일을 검색하는 다단계 감염 체인을 시작합니다. 지속성은 기본 payl 가져오기 및 실행을 담당하는 CAT 파일을 시작하도록 구성된 예약된 작업을 통해 달성됩니다.디스크에 어떤 아티팩트도 남기지 않고 메모리에 로드합니다.