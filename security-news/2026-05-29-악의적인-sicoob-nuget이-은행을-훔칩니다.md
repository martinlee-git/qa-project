# 악의적인 Sicoob Nuget이 은행을 훔칩니다.
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/05/malicious-sicoob-nuget-steals-banking.html
- Published At: unknown
- Collected At: 2026-05-29T13:06:02.968Z
- Notion Page: https://www.notion.so/The-Hacker-News-Sicoob-Nuget-36ffc93aec5781398a6afbb7baf2de57
- Original Title: Malicious Sicoob Nuget Steals Banking
## Summary
악성 Sicoob.Sdk는 NuGet 다운로드를 통해 PFX 인증서와 클라이언트 ID를 훔쳐 API 가장 및 결제 남용 위험을 발생시켰습니다. 사이버 보안 연구원들이 브라질 최대 협력 금융 시스템 중 하나인 Sicoob용 C# 소프트웨어 개발 키트로 가장하여 클라이언트 ID와 PFX 인증서를 빼내는 악성 NuGet 패키지를 발견했습니다. Socket에 따르면 "Sicoob.Sdk" 버전 2.0.0~2.0.4에는 즉시 결제 처리 및 동적 Pix QR 코드 생성과 같은 은행 운영을 자동화하기 위해 Sicoob 뱅킹 네트워크로 기업을 인증하는 데 사용되는 PFX 인증서를 포함하여 민감한 정보를 추출하는 기능이 포함되어 있습니다.

## Original Description

Malicious Sicoob.Sdk stole PFX certificates and client IDs via NuGet downloads, enabling API impersonation and payment abuse risks.
## Key Points
- 악성 Sicoob.Sdk는 NuGet 다운로드를 통해 PFX 인증서와 클라이언트 ID를 훔쳐 API 가장 및 결제 남용 위험을 발생시켰습니다.
- 사이버 보안 연구원들이 브라질 최대 협력 금융 시스템 중 하나인 Sicoob용 C# 소프트웨어 개발 키트로 가장하여 클라이언트 ID와 PFX 인증서를 빼내는 악성 NuGet 패키지를 발견했습니다.
- Socket에 따르면 "Sicoob.Sdk" 버전 2.0.0~2.0.4에는 즉시 결제 처리 및 동적 Pix QR 코드 생성과 같은 은행 운영을 자동화하기 위해 Sicoob 뱅킹 네트워크로 기업을 인증하는 데 사용되는 PFX 인증서를 포함하여 민감한 정보를 유출하는 기능이 포함되어 있습니다.
## Excerpt
사이버 보안 연구원들이 브라질 최대 협력 금융 시스템 중 하나인 Sicoob용 C# 소프트웨어 개발 키트로 가장하여 클라이언트 ID와 PFX 인증서를 빼내는 악성 NuGet 패키지를 발견했습니다. Socket에 따르면 "Sicoob.Sdk" 버전 2.0.0~2.0.4에는 즉시 결제 처리 및 동적 Pix QR 코드 생성과 같은 은행 운영을 자동화하기 위해 Sicoob 뱅킹 네트워크로 기업을 인증하는 데 사용되는 PFX 인증서를 포함하여 민감한 정보를 유출하는 기능이 포함되어 있습니다. 해당 패키지는 거의 500회 다운로드된 것으로 추정됩니다. 보안 연구원인 Kirill Boychenko는 "개발자가 클라이언트 ID, PFX 파일 경로 및 PFX 비밀번호를 사용하여 SicoobClient를 인스턴스화하면 패키지는 디스크에서 PFX 파일을 읽고 해당 내용을 Base64로 인코딩한 다음 제공된 클라이언트 ID, PFX 비밀번호 및 인코딩된 PFX 데이터를 하드코딩된 타사 Sentry 엔드포인트로 보냅니다."라고 말했습니다. 또한 이 패키지는 별도의 Sentry 경로를 통해 원시 Boleto API 응답을 캡처하도록 설계되었습니다. Boleto는 브라질에서 온라인 및 오프라인 구매 시 널리 사용되는 현금 결제 수단입니다. 이로 인해 민감한 거래 세부정보, 결제 상태, 금액, 만기일, 식별자, 지급인 또는 수취인 데이터가 노출될 가능성이 있습니다. 결과적으로 도난당한 데이터는 위협 행위자가 피해자의 Sicoob 뱅킹 API 통합을 가장하기 위해 악용할 수 있기 때문에 심각한 위험에 노출될 수 있다고 Socket은 덧붙였습니다. 책임 있는 공개에 따름e, 패키지가 NuGet에 의해 차단되었습니다. "sicoob"이라는 패키지 뒤에 있는 프로필에는 전체적으로 약 6,000번의 다운로드를 기록한 11개의 다른 NuGet 패키지도 나열되어 있습니다.