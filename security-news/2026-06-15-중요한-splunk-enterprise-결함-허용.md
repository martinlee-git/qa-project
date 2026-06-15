# 중요한 Splunk Enterprise 결함 허용
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/critical-splunk-enterprise-flaw-lets.html
- Published At: unknown
- Collected At: 2026-06-15T08:44:47.602Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Splunk-Enterprise-37efc93aec5781aca5cbe105581c0779
- Original Title: Critical Splunk Enterprise Flaw Lets
## Summary
Splunk는 인증되지 않은 원격 코드 실행을 허용하는 Splunk Enterprise의 중요한 CVSS 9.8 취약점에 대한 보안 업데이트를 발표했습니다. Splunk는 인증되지 않은 파일 작업은 물론 원격 코드 실행까지 악용할 수 있는 Splunk Enterprise의 심각한 보안 결함을 해결하기 위해 보안 업데이트를 출시했습니다. CVE-2026-20253 으로 추적되는 이 취약점은 CVSS 채점 시스템에서 9.8 등급을 받았습니다. Splunk는 이번 주 경고를 통해 "10.2.4 및 10.0.7 이하의 Splunk Enterprise 버전에서는 인증되지 않은 사용자가 PostgreSQL 사이드카 서비스 엔드포인트를 통해 임의의 파일을 생성하거나 자를 수 있습니다"라고 밝혔습니다. "이 취약점은 PostgreSQL 사이드카 서비스 엔드포인트 때문에 존재합니다…

## Original Description

Splunk issued security updates for a critical CVSS 9.8 vulnerability in Splunk Enterprise that allows unauthenticated remote code execution.
## Key Points
- Splunk는 인증되지 않은 원격 코드 실행을 허용하는 Splunk Enterprise의 중요한 CVSS 9.8 취약점에 대한 보안 업데이트를 발표했습니다.
- Splunk는 인증되지 않은 파일 작업은 물론 원격 코드 실행까지 악용할 수 있는 Splunk Enterprise의 심각한 보안 결함을 해결하기 위해 보안 업데이트를 출시했습니다.
- CVE-2026-20253 으로 추적되는 이 취약점은 CVSS 채점 시스템에서 9.8 등급을 받았습니다.
## Excerpt
Splunk는 인증되지 않은 파일 작업은 물론 원격 코드 실행까지 악용할 수 있는 Splunk Enterprise의 심각한 보안 결함을 해결하기 위해 보안 업데이트를 출시했습니다. CVE-2026-20253 으로 추적되는 이 취약점은 CVSS 채점 시스템에서 9.8 등급을 받았습니다. Splunk는 이번 주 경고를 통해 "10.2.4 및 10.0.7 이하의 Splunk Enterprise 버전에서는 인증되지 않은 사용자가 PostgreSQL 사이드카 서비스 엔드포인트를 통해 임의의 파일을 생성하거나 자를 수 있습니다"라고 밝혔습니다. "이 취약점은 PostgreSQL 사이드카 서비스 엔드포인트에 인증 제어 기능이 부족하여 네트워크에 연결할 수 있는 모든 사용자가 자격 증명 없이 파일 작업을 호출할 수 있기 때문에 존재합니다." 이 문제는 다음 버전에서 해결되었습니다.