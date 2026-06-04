# 언어, 도메인 또는 악센트에 맞게 Nemotron 3.5 ASR을 미세 조정하는 방법
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/nvidia/fine-tuning-nemotron-35-asr
- Published At: Thu, 04 Jun 2026 12:59:35 GMT
- Collected At: 2026-06-04T15:50:53.685Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-Nemotron-3-5-ASR-375fc93aec5781f6a337d18fe07f9f0f
- Original Title: How to Fine-Tune Nemotron 3.5 ASR for Your Language, Domain, or Accent
## Summary
Hugging Face에 대한 NVIDIA의 블로그 게시물 현재 다국어 음성 인식의 문제점 작동 방식 작동 방식(2분 버전) att_context_size</code>"> 알아둘 만한 손잡이: att_context_size 몇 분 만에 시도 미세 조정이 필요한 이유 미세 조정의 힘 미리 보기 레시피 개요 1단계 — 데이터 2단계 — 훈련 3단계 — 평가 4단계 — 도움이 되는 방향으로 데이터 확장 5단계 — 배포 대상 학습할 수 있는 것 시작하기 NVIDIA Nemotron 3.5 ASR 소개, 다국어 스트리밍: 단일 체크포인트에서 40개의 언어 로케일을 실시간으로 기록하고 구두점과 대문자를 내장한 600M 매개변수 음성-텍스트 모델입니다.

## Original Description

A Blog post by NVIDIA on Hugging Face
## Key Points
- Hugging Face에 대한 NVIDIA의 블로그 게시물 오늘날 다국어 음성 인식의 문제점 기능 작동 방식(2분 버전) att_context_size</code>"> 알아둘 만한 손잡이: att_context_size 몇 분 만에 시도해 보세요 왜 미세 조정해야 할까요?
- 미세 조정의 힘 미리 보기 레시피 개요 1단계 — 데이터 2단계 — 훈련 3단계 — 평가 4단계 — 도움이 되는 곳에 데이터 확장 5단계 — 배운 내용 배포 이를 통해 구축할 수 있는 것 시작하기 다국어 스트리밍 NVIDIA Nemotron 3.5 ASR 소개: 단일 체크포인트에서 40개 언어 로케일을 실시간으로 기록하는 600M 매개변수 음성-텍스트 모델 , 구두점과 대문자가 내장되어 있습니다.
- 올해 초 Hugging Face와 NIM으로 출시된 인기 Nemotron 3 ASR 모델(영어로만 제공)의 후속 제품입니다.
## Excerpt
현재 다국어 음성 인식의 문제점 기능 작동 방식(2분 버전) att_context_size</code>"> 알 만한 가치가 있는 손잡이: att_context_size 몇 분 안에 시도해 보십시오. 미세 조정이 필요한 이유 미세 조정의 힘 미리 보기 한 눈에 보는 레시피 1단계 — 데이터 2단계 — 훈련 3단계 — 평가 4단계 — 도움이 되는 방향으로 데이터 확장 5단계 — 배운 내용 배포 이를 통해 구축할 수 있는 것 시작하기 NVIDIA Nemotron 3.5 ASR 소개, 다국어 스트리밍: 단일 체크포인트에서 40개의 언어 로케일을 실시간으로 기록하고 구두점과 대문자를 내장한 600M 매개변수 음성-텍스트 모델입니다. Nemotron 3 ASR은 올해 초 Hugging Face에서 NIM으로 출시된 인기 있는 Nemotron 3 ASR 모델(영어만 해당)의 후속 모델입니다. 인공 분석(Artificial Analysis)의 독립적인 벤치마크에 의해 검증되었습니다. 모든 스트리밍 ASR 모델 중 지연 시간이 2위(음성 종료 후 최종 기록까지 단 0.07초)이며 AA-WER 스트리밍 지수와 최종 전사까지의 시간 순위표에서 "가장 매력적인 사분면"에 위치하여 정확도-지연 시간 균형을 결합한 최고의 모델 중 하나입니다. 이 모델은 중복 없이 오디오를 스트리밍하는 캐시 인식 FastConformer-RNNT 아키텍처를 사용합니다. 대부분의 스트리밍 ASR을 느리게 만드는 재계산 — Nemotron 3.5 ASR은 Hugging Face에서 개방형 가중치로 제공되므로 낮은 대기 시간과 높은 정확도를 얻을 수 있습니다.API 종속성이나 호출별 청구 없이 이를 검사하고, 세부 조정하고, 배포할 수 있습니다. 귀하가 선택하지 않는 한 데이터는 인프라를 떠나지 않습니다. 강력한 기본 모델이므로 자신의 언어, 도메인 또는 억양에 맞게 세부 조정할 수 있습니다. 이 게시물의 후반부에서는 정확한 방법을 안내합니다. 만약에…