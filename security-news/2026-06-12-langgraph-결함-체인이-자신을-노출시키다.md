# Langgraph 결함 체인이 자신을 노출시키다
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/langgraph-flaw-chain-exposes-self.html
- Published At: unknown
- Collected At: 2026-06-12T18:01:47.464Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Langgraph-37dfc93aec5781d899d1d581ea84904e
- Original Title: Langgraph Flaw Chain Exposes Self
## Summary
세 가지 패치된 LangGraph 결함으로 인해 공격자는 자체 호스팅 배포에서 RCE에 대해 SQL 주입 및 안전하지 않은 역직렬화를 연결할 수 있습니다. 사이버 보안 연구원들은 원격 코드 실행을 초래할 수 있는 중요한 취약점 체인을 포함하여 현재 패치된 LangGraph에 영향을 미치는 세 가지 보안 결함에 대한 세부 정보를 공개했습니다. LangGraph는 복잡한 상태 저장 다중 에이전트 인공 지능(AI) 에이전트 애플리케이션을 구축하기 위해 LangChain에서 만든 오픈 소스 프레임워크입니다. Check Point는 "LangGraph 기능에 SQL을 주입하면 시스템이 데이터를 처리하고 처리하는 방식의 약점을 이용하여 공격자가 서버의 원격 코드 실행을 통해 완전한 제어권을 얻을 수 있습니다"라고 말했습니다. 리…

## Original Description

Three patched LangGraph flaws could let attackers chain SQL injection and unsafe deserialization for RCE in self-hosted deployments.
## Key Points
- 세 가지 패치된 LangGraph 결함으로 인해 공격자는 자체 호스팅 배포에서 RCE에 대해 SQL 주입 및 안전하지 않은 역직렬화를 연결할 수 있습니다.
- 사이버 보안 연구원들은 원격 코드 실행을 초래할 수 있는 중요한 취약점 체인을 포함하여 현재 패치된 LangGraph에 영향을 미치는 세 가지 보안 결함에 대한 세부 정보를 공개했습니다.
- LangGraph는 복잡한 상태 저장 다중 에이전트 인공 지능(AI) 에이전트 애플리케이션을 구축하기 위해 LangChain에서 만든 오픈 소스 프레임워크입니다.
## Excerpt
사이버 보안 연구원들은 원격 코드 실행을 초래할 수 있는 중요한 취약점 체인을 포함하여 현재 패치된 LangGraph에 영향을 미치는 세 가지 보안 결함에 대한 세부 정보를 공개했습니다. LangGraph는 복잡한 상태 저장 다중 에이전트 인공 지능(AI) 에이전트 애플리케이션을 구축하기 위해 LangChain에서 만든 오픈 소스 프레임워크입니다. Check Point는 "LangGraph 기능에 SQL을 주입하면 시스템이 데이터를 처리하고 처리하는 방식의 약점을 이용하여 공격자가 서버의 원격 코드 실행을 통해 완전한 제어권을 얻을 수 있습니다"라고 말했습니다. 확인된 취약점 목록은 다음과 같습니다. "취약점 체인은 사용자 제어 필터 입력이 있는 SQLite 또는 Redis 체크포인터를 사용하는 자체 호스팅 배포에서 악용될 수 있습니다."라고 Check Point는 말했습니다. "LangChain의 관리형 플랫폼(LangSmith 배포)은 영향을 받지 않습니다."