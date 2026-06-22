# MolmoMotion: 언어 기반 3D 모션 예측
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/allenai/molmomotion
- Published At: Wed, 17 Jun 2026 15:26:44 GMT
- Collected At: 2026-06-22T10:46:38.082Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-MolmoMotion-3D-382fc93aec578148a22ac54f9ef84cff
- Original Title: MolmoMotion: Language-guided 3D motion forecasting
## Summary
Hugging Face MolmoMotion에 대한 Ai2의 블로그 게시물: 내부 MolmoMotion-1M 및 PointMotionBench 소개 실험 및 성능 3D 모션 예측 다운스트림 평가: 로봇 공학 계획 다운스트림 평가: 비디오 생성 제한 사항 및 향후 계획 🧠 모델: https://huggingface.co/collections/allenai/molmomotion | 📄 기술 보고서: https://allenai.org/papers/molmomotion | 📊 데이터: https://huggingface.co/datasets/allenai/molmo-motion-1m | 💻 코드: https://github.com/allenai/molmo-motion.git | 🌐 프로젝트 페이지: https://molmomotion.github.io/ 기계는 동작을 인식하는 데 놀라울 정도로 능숙해졌습니다. 비디오가 제공되면 현대 모델은 물체와 점이 어떻게 이동하는지 추적할 수 있습니다.

## Original Description

A Blog post by Ai2 on Hugging Face
## Key Points
- Hugging Face MolmoMotion에 대한 Ai2의 블로그 게시물: 내부 MolmoMotion-1M 및 PointMotionBench 소개 실험 및 성능 3D 모션 예측 다운스트림 평가: 로봇 공학 계획 다운스트림 평가: 비디오 생성 제한 사항 및 향후 계획 🧠 모델: https://huggingface.co/collections/allenai/molmomotion | 📄 기술 보고서: https://allenai.org/papers/molmomotion | 📊 데이터: https://huggingface.co/datasets/allenai/molmo-motion-1m | 💻 코드: https://github.com/allenai/molmo-motion.git | 🌐 프로젝트 페이지: https://molmomotion.github.io/ 기계는 동작을 인식하는 데 놀라울 정도로 능숙해졌습니다.
- 비디오가 제공되면 현대 모델은 매우 높은 신뢰도로 장면에서 물체와 점이 어떻게 움직이는지 추적할 수 있습니다.
- 그러나 지각은 본질적으로 회고적입니다. 이미 발생한 움직임을 설명합니다.
## Excerpt
MolmoMotion: 내부 MolmoMotion-1M 및 PointMotionBench 소개 실험 및 성능 3D 모션 예측 다운스트림 평가: 로봇 공학 계획 다운스트림 평가: 비디오 생성 제한 사항 및 향후 계획 🧠 모델: https://huggingface.co/collections/allenai/molmomotion | 📄 기술 보고서: https://allenai.org/papers/molmomotion | 📊 데이터: https://huggingface.co/datasets/allenai/molmo-motion-1m | 💻 코드: https://github.com/allenai/molmo-motion.git | 🌐 프로젝트 페이지: https://molmomotion.github.io/ 기계는 동작을 인식하는 데 놀라울 정도로 능숙해졌습니다. 비디오가 제공되면 현대 모델은 매우 높은 신뢰도로 장면에서 물체와 점이 어떻게 움직이는지 추적할 수 있습니다. 그러나 지각은 본질적으로 회고적입니다. 이미 발생한 움직임을 설명합니다. 우리가 구축하려는 많은 시스템과 애플리케이션은 대신 미래를 내다볼 필요가 있습니다. 컵을 향해 손을 뻗는 로봇은 컵이 컵에 닿기 전에 컵이 어떻게 움직일지 예측해야 합니다. 비디오 생성기는 물리적으로 그럴듯한 프레임을 생성하려면 다음에 어떤 현실적인 모션이 나올지 알아야 합니다. 동작을 예측하는 것은 관찰하는 것보다 어렵지만 많은 시나리오에서 훨씬 더 유용합니다. 이 아이디어는 우리가 오늘 출시하는 새로운 동작 예측 모델인 MolmoMotion의 동기가 되었습니다. 비디오 프레임, 물체에 표시된 3D 점, 의도된 동작을 설명하는 서면 지침(예: "테이블 위에 과일이 담긴 나무 그릇을 움직이고 회전하세요")이 주어지면 MolmoMotion은 해당 지점이 어디에 있는지 예측합니다.ts는 3D 공간에서 다음 몇 초 동안 이동하여 기존 예측 방법보다 훨씬 더 강력한 성능을 달성합니다. RGB 관찰, 객체의 쿼리 포인트 세트 및 동작 설명이 주어지면 MolmoMotion은 객체의 미래 3D 포인트 궤적을 예측합니다. 이러한 예측은…