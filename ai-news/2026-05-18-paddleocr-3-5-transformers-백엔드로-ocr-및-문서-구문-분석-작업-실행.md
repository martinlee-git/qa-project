# PaddleOCR 3.5: Transformers 백엔드로 OCR 및 문서 구문 분석 작업 실행
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/PaddlePaddle/paddleocr-transformers
- Published At: Mon, 18 May 2026 15:12:46 GMT
- Collected At: 2026-05-25T15:57:01.122Z
- Notion Page: https://www.notion.so/Hugging-Face-Blog-PaddleOCR-3-5-Transformers-OCR-36bfc93aec5781c3b6fbfe69e7869da9
- Original Title: PaddleOCR 3.5: Running OCR and Document Parsing Tasks with a Transformers Backend
## Summary
Hugging Face에 대한 PaddlePaddle의 블로그 게시물 무엇이 바뀌었나요? 이것이 중요한 이유 빠른 시작 언제 Transformers 백엔드를 사용해야 합니까? 지금 사용해 보세요 리소스 감사패 PaddleOCR 3.5는 OCR 및 문서 구문 분석 작업을 Hugging Face 생태계에 더 가깝게 만듭니다. 이 릴리스에서 지원되는 PaddleOCR 모델은 다음 설정을 통해 Hugging Face Transformers를 추론 백엔드로 실행할 수 있습니다. PaddleOCR은 PP-OCRv5와 같은 OCR 모델 시리즈 및 PaddleOCR-VL 1.5와 같은 문서 구문 분석 모델 시리즈를 계속 제공하는 반면 Transformers는 이를 실행하기 위해 지원되는 백엔드 중 하나가 됩니다. Hugging Face Spaces의 라이브 데모를 사용해 보세요: https://huggingface.co/spaces/PaddlePaddle/paddleocr-3.5-transformers-demo…

## Original Description

A Blog post by PaddlePaddle on Hugging Face
## Key Points
- Hugging Face에 대한 PaddlePaddle의 블로그 게시물 무엇이 바뀌었나요?
- 이것이 중요한 이유 빠른 시작 언제 Transformers 백엔드를 사용해야 합니까?
- 지금 사용해 보세요 리소스 감사패 PaddleOCR 3.5는 OCR 및 문서 구문 분석 작업을 Hugging Face 생태계에 더 가깝게 만듭니다.
## Excerpt
무엇이 바뀌었나요? 이것이 중요한 이유 빠른 시작 언제 Transformers 백엔드를 사용해야 합니까? 지금 사용해 보세요 리소스 감사패 PaddleOCR 3.5는 OCR 및 문서 구문 분석 작업을 Hugging Face 생태계에 더 가깝게 만듭니다. 이 릴리스에서 지원되는 PaddleOCR 모델은 다음 설정을 통해 Hugging Face Transformers를 추론 백엔드로 실행할 수 있습니다. PaddleOCR은 PP-OCRv5와 같은 OCR 모델 시리즈 및 PaddleOCR-VL 1.5와 같은 문서 구문 분석 모델 시리즈를 계속 제공하는 반면 Transformers는 이를 실행하기 위해 지원되는 백엔드 중 하나가 됩니다. Hugging Face Spaces의 라이브 데모를 사용해 보세요: https://huggingface.co/spaces/PaddlePaddle/paddleocr-3.5-transformers-demo PaddleOCR 3.5는 보다 유연한 추론 엔진 인터페이스를 도입합니다. 개발자는 엔진 매개변수를 통해 백엔드를 선택하고,engine_config를 통해 백엔드별 옵션을 전달할 수 있습니다. 이번 릴리스는 주로 추론 백엔드 계층에 관한 것입니다. PaddleOCR은 OCR 및 문서 구문 분석 기능을 계속 제공하는 반면 Transformers는 지원되는 PaddleOCR 모델에 Hugging Face 중심 환경에 자연스럽게 맞는 또 다른 백엔드 옵션을 제공합니다. 더 큰 Document AI 워크플로는 여전히 개발자와 애플리케이션 빌더의 손에 있습니다.