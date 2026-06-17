# Hugging Face Hub부터 Strands Agents 및 LeRobot을 갖춘 로봇 하드웨어까지
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/amazon/strands-lerobot-hub-to-hardware
- Published At: Wed, 17 Jun 2026 10:18:05 GMT
- Collected At: 2026-06-17T11:20:41.553Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-Hugging-Face-Hub-Strands-Agents-LeRobot-382fc93aec57810d9bd5e52cac309d61
- Original Title: From the Hugging Face Hub to robot hardware with Strands Agents and LeRobot
## Summary
Hugging Face에 대한 Amazon의 블로그 게시물 구축할 내용 전제 조건 1단계 - 예제 설정 2단계 - 데모 기록 및 허브에 푸시 3단계 - 시뮬레이션에서 정책 실행 4단계 - 물리적 하드웨어에 정책 배포 5단계 - 여러 로봇을 메시와 조정 샘플 애플리케이션을 사용하여 시도 보안 고려 사항 정리 이것이 서로 맞는 방법 여기에서 갈 곳 리소스 작성자 Strands Robots의 LeRobot 통합에 대한 연습 - 하나의 에이전트 루프에서 동일한 온디스크 형식의 시뮬레이션-실제 데이터세트와 문자열로 교환하는 정책을 사용하여 데이터세트를 물리적 로봇에 허브합니다. Hugging Face Hub에 데모 데이터 폴더인 로봇이 있습니다.

## Original Description

A Blog post by Amazon on Hugging Face
## Key Points
- Hugging Face에 대한 Amazon의 블로그 게시물 구축할 내용 전제 조건 1단계 - 예제 설정 2단계 - 데모 기록 및 허브에 푸시 3단계 - 시뮬레이션에서 정책 실행 4단계 - 물리적 하드웨어에 정책 배포 5단계 - 여러 로봇을 메시와 조정 샘플 애플리케이션을 사용하여 시도 보안 고려 사항 정리 이것이 서로 맞는 방법 여기에서 갈 곳 리소스 작성자 Strands Robots의 LeRobot 통합에 대한 연습 - 하나의 에이전트 루프에서 동일한 온디스크 형식의 시뮬레이션-실제 데이터세트와 문자열로 교환하는 정책을 사용하여 데이터세트를 물리적 로봇에 허브합니다.
- Hugging Face Hub에 로봇, 데모 데이터 폴더, 그리고 로봇이 배우기를 원하는 새로운 작업이 있습니다.
- 오늘날 이를 위해서는 다섯 가지 별도의 도구가 필요합니다. 하나는 새로운 데모를 기록하기 위한 도구, 다른 하나는 교육용 도구, 세 번째는 시뮬레이션에서 테스트하기 위한 도구, 하드웨어에 배포하기 위한 사용자 정의 코드, 로봇이 두 대 이상일 때 조정하기 위한 도구입니다.
## Excerpt
구축할 내용 전제 조건 1단계 - 예제 설정 2단계 - 데모 기록 및 허브에 푸시 3단계 - 시뮬레이션에서 정책 실행 4단계 - 물리적 하드웨어에 정책 배포 5단계 - 여러 로봇을 메시로 조정 샘플 애플리케이션을 사용하여 시도 보안 고려 사항 정리 여기에서 이동하는 방법 리소스 작성자 Strands Robots의 LeRobot 통합에 대한 연습 - 허브 데이터 세트에서 물리적 로봇까지의 하나의 에이전트 루프 동일한 온디스크 형식의 시뮬레이션-실제 데이터 세트와 문자열로 바꾸는 정책. Hugging Face Hub에 로봇, 데모 데이터 폴더, 그리고 로봇이 배우기를 원하는 새로운 작업이 있습니다. 오늘날 이를 위해서는 다섯 가지 별도의 도구가 필요합니다. 하나는 새로운 데모를 기록하기 위한 도구, 다른 하나는 교육용 도구, 세 번째는 시뮬레이션에서 테스트하기 위한 도구, 하드웨어에 배포하기 위한 사용자 정의 코드, 로봇이 두 대 이상일 때 조정하기 위한 도구입니다. 작품은 스스로 작동합니다. 그들은 서로 이야기하지 않습니다. Strands Robots는 로봇 추상화, 시뮬레이션 및 LeRobot 스택을 단일 Strands 에이전트로 구성하는 AgentTools로 표시하는 AWS(Apache 2.0)의 오픈 소스 SDK입니다. 통합은 의도적으로 얇습니다. LeRobot의 자체 스크립트는 하드웨어 기록 및 교정을 처리하고 Strands AgentTools는 에이전트가 실제로 조정하는 부분에 사용됩니다. 시뮬레이션 도구는 LeRobot이 하드웨어에 쓰는 것과 동일한 형식으로 LeRobotDatasets를 기록합니다. GR00T 및 LerobotLocal은 통신 뒤에 정책 추론을 제공합니다.인터페이스에서, MolmoAct2 체크포인트는 LerobotLocal 경로를 통해 실행됩니다. 피어 메시는 에이전트를 원격 로봇으로 팬아웃합니다. 데이터 세트 형식은 LeRobot이 작성한 그대로 유지됩니다. 에이전트 루프는 접착제입니다. 이 게시물은 단일 에이전트 내부의 5단계를 안내합니다. LeRobo 위에 에이전트를 구축합니다…