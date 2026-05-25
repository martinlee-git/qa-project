# Ettin Reranker 제품군 소개
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/ettin-reranker
- Published At: Tue, 19 May 2026 00:00:00 GMT
- Collected At: 2026-05-25T15:57:00.755Z
- Notion Page: https://www.notion.so/Hugging-Face-Blog-Ettin-Reranker-36bfc93aec5781109aa0c6a8ba27eb81
- Original Title: Introducing the Ettin Reranker Family
## Summary
우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다. 오늘 저는 Ettin ModernBERT 인코더를 기반으로 구축된 각 크기의 최신 Sentence Transformers CrossEncoder reranker 6개를 이를 생성한 데이터 및 전체 교육 레시피와 함께 출시합니다. 모델은 증류 레시피로 교육되었습니다. lightonai/embeddings-pre-training의 하위 집합과 lightonai/embeddings-fine-tuning의 순위가 변경된 하위 집합이 혼합되어 있습니다. MTEB(eng, v2) Retri에서 google/embeddinggemma-300m과 짝을 이루는 6명의 reranker…

## Original Description

We’re on a journey to advance and democratize artificial intelligence through open source and open science.
## Key Points
- 우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다.
- 오늘 저는 Ettin ModernBERT 인코더를 기반으로 구축된 각 크기의 최신 Sentence Transformers CrossEncoder reranker 6개를 이를 생성한 데이터 및 전체 교육 레시피와 함께 출시합니다. 모델은 증류 레시피로 교육되었습니다. lightonai/embeddings-pre-training의 하위 집합과 lightonai/embeddings-fine-tuning의 순위가 변경된 하위 집합이 혼합되어 있습니다.
- MTEB(eng, v2) 검색에서 google/embeddinggemma-300m과 쌍을 이루는 6개의 reranker입니다.
## Excerpt
오늘 저는 Ettin ModernBERT 인코더를 기반으로 구축된 각 크기의 최신 Sentence Transformers CrossEncoder reranker 6개를 이를 생성한 데이터 및 전체 교육 레시피와 함께 출시합니다. 모델은 증류 레시피로 교육되었습니다. lightonai/embeddings-pre-training의 하위 집합과 lightonai/embeddings-fine-tuning의 순위가 변경된 하위 집합이 혼합되어 있습니다. MTEB(eng, v2) 검색에서 google/embeddinggemma-300m과 쌍을 이루는 6개의 reranker입니다. 5개의 추가 임베더 쌍에 대해서는 결과를 참조하세요. reranker를 처음 사용하고 "이유"를 먼저 알고 싶다면 reranker란 무엇이며 임베더와 쌍을 이루는 이유는 무엇입니까?로 이동하세요. . 모델을 연결하고 싶다면 사용법으로 이동하세요. 직접 훈련하려면 훈련 으로 이동하세요. Sentence Transformers v5.5.0에 제공된 새로운 train-sentence-transformers Agent Skill을 사용하여 아래 교육 레시피를 부트스트랩했습니다. hf Skills add train-sentence-transformers [--global] [--claude]와 함께 설치하고 AI 코딩 에이전트(Claude Code, Codex, Cursor, Gemini CLI, ...)에게 데이터에 대한 SentenceTransformer, CrossEncoder 또는 SparseEncoder 모델을 미세 조정하도록 요청하세요.