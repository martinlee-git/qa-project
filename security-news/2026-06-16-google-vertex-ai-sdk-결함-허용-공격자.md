# Google Vertex Ai SDK 결함 허용 공격자
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/google-vertex-ai-sdk-flaw-let-attackers.html
- Published At: unknown
- Collected At: 2026-06-16T20:10:42.896Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Google-Vertex-Ai-SDK-381fc93aec5781a587dae244a82845be
- Original Title: Google Vertex Ai Sdk Flaw Let Attackers
## Summary
Google은 Unit 42에서 버킷 스쿼트를 통해 모델 하이재킹 및 코드 실행이 가능하다는 사실을 확인한 후 v1.148.0의 Vertex AI SDK 결함을 수정했습니다. Python용 Google Cloud Vertex AI SDK의 결함으로 인해 피해자의 프로젝트에 액세스할 수 없는 공격자가 피해자의 기계 학습 모델 업로드를 가로채고 Google 서비스 인프라 내에서 코드를 실행할 수 있습니다. 구글의 버그 바운티 프로그램을 통해 버그를 발견해 보고한 팔로알토 네트웍스 유닛 42는 이 기술을 '피클 인 더 미들(Pickle in the Middle)'이라고 부르며, 실제로는 악용 사례가 발견되지 않았다고 밝혔다. Google이 이를 패치했습니다. SDK를 사용하는 경우 버전 1.148.0 이상으로 업데이트하세요. 공격자는 자신의 Google Cloud 프로젝트와 피해자의 프로젝트 ID만 있으면 됩니다.

## Original Description

Google fixed a Vertex AI SDK flaw in v1.148.0 after Unit 42 showed bucket squatting could enable model hijacking and code execution.
## Key Points
- Google은 Unit 42에서 버킷 스쿼트를 통해 모델 하이재킹 및 코드 실행이 가능하다는 사실을 확인한 후 v1.148.0의 Vertex AI SDK 결함을 수정했습니다.
- Python용 Google Cloud Vertex AI SDK의 결함으로 인해 피해자의 프로젝트에 액세스할 수 없는 공격자가 피해자의 기계 학습 모델 업로드를 가로채고 Google 서비스 인프라 내에서 코드를 실행할 수 있습니다.
- 구글의 버그 바운티 프로그램을 통해 버그를 발견해 보고한 팔로알토 네트웍스 유닛 42는 이 기술을 '피클 인 더 미들(Pickle in the Middle)'이라고 부르며, 실제로는 악용 사례가 발견되지 않았다고 밝혔다.
## Excerpt
Python용 Google Cloud Vertex AI SDK의 결함으로 인해 피해자의 프로젝트에 액세스할 수 없는 공격자가 피해자의 기계 학습 모델 업로드를 가로채고 Google 서비스 인프라 내에서 코드를 실행할 수 있습니다. 구글의 버그 바운티 프로그램을 통해 버그를 발견해 보고한 팔로알토 네트웍스 유닛 42는 이 기술을 '피클 인 더 미들(Pickle in the Middle)'이라고 부르며, 실제로는 악용 사례가 발견되지 않았다고 밝혔다. Google이 이를 패치했습니다. SDK를 사용하는 경우 버전 1.148.0 이상으로 업데이트하세요. 공격자에게는 자체 Google Cloud 프로젝트와 공개되는 경우가 많은 피해자의 프로젝트 ID만 필요했습니다. 자격 증명도 없고, 피싱도 없고, 대상에 발판도 없습니다. 결함은 SDK가 모델 업로드를 위해 임시 Cloud Storage 버킷을 선택하는 방식에 있었습니다. 사용자가 버킷을 설정하지 않은 경우 SDK는 프로젝트 ID 및 지역에서 project-vertex-staging-region 과 같은 예측 가능한 이름을 생성했습니다. 해당 버킷이 존재하는지 확인했지만 피해자가 이를 소유했는지 여부는 확인하지 않았습니다. 버킷 이름은 전역적으로 고유하므로 공격자는 자신의 프로젝트에서 예상되는 버킷을 먼저 생성할 수 있습니다. 그러면 피해자의 SDK가 모델 파일을 공격자의 버킷에 업로드합니다. 그런 다음 공격자는 업로드된 모델을 악성 모델로 교체할 수 있습니다.