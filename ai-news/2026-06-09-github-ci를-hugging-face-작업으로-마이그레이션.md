# GitHub CI를 Hugging Face 작업으로 마이그레이션
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/github-ci-hf-jobs
- Published At: Tue, 09 Jun 2026 00:00:00 GMT
- Collected At: 2026-06-10T13:30:48.969Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-GitHub-CI-Hugging-Face-37afc93aec57813da91ef81440e769b4
- Original Title: Migrating Your GitHub CI to Hugging Face Jobs
## Summary
우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다. 허깅페이스 채용이란? 아키텍처 1단계: 디스패처 공간 복제 2단계: GitHub 앱 웹 설정 생성 및 설치 에이전트 지원 설정 3단계: 최종 디스패처 설정 실행</code>"> 4단계: 실행 변경 5단계: 테스트 결과 GitHub 리포지토리가 있고 GitHub Actions가 활성화된 경우 CI용 GitHub 호스팅 실행기를 사용할 가능성이 높습니다. 이는 간단하기 때문에 많은 프로젝트의 기본값입니다. 워크플로 추가, 실행: ubuntu-latest 작성, GitHub는 머신을 제공합니다. 이 기본값은 편리하지만 GitHub Actions는 속도가 느릴 수도 있습니다.

## Original Description

We’re on a journey to advance and democratize artificial intelligence through open source and open science.
## Key Points
- 우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다.
- 허깅페이스 채용이란?
- 아키텍처 1단계: 디스패처 공간 복제 2단계: GitHub 앱 웹 설정 생성 및 설치 에이전트 지원 설정 3단계: 최종 디스패처 설정 실행</code>"> 4단계: 실행 변경 5단계: 테스트 결과 GitHub 저장소가 있고 GitHub Actions가 활성화된 경우 CI용 GitHub 호스팅 실행기를 사용할 가능성이 높습니다.
## Excerpt
허깅페이스 채용이란? 아키텍처 1단계: 디스패처 공간 복제 2단계: GitHub 앱 웹 설정 생성 및 설치 에이전트 지원 설정 3단계: 최종 디스패처 설정 실행</code>"> 4단계: 실행 변경 5단계: 테스트 결과 GitHub 리포지토리가 있고 GitHub Actions가 활성화된 경우 CI용 GitHub 호스팅 실행기를 사용할 가능성이 높습니다. 이는 간단하기 때문에 많은 프로젝트의 기본값입니다. 워크플로 추가, 실행: ubuntu-latest 작성, GitHub Actions는 유지 관리를 위해 속도가 느려지거나 느려질 수 있으며 GPU 액세스는 대부분의 오픈 소스 프로젝트에서 사용할 수 있는 것이 아닙니다. Trackio의 경우 이러한 제한이 중요해지기 시작했습니다. 우리는 실제 CUDA 하드웨어에서 실행해야 하는 테스트를 위한 GPU CI도 원했습니다. 결과: Trackio의 CI는 이제 Hugging Face Jobs에서 실행되고 실시간 로그를 다시 스트리밍하여 CPU 작업에 대한 CI 시간을 약 30% 단축하고 GPU 시스템에서 실행되는 완전히 새로운 테스트 제품군을 활성화합니다. 이 문서에서는 GitHub 저장소에 대해 동일한 설정을 다시 만드는 방법을 단계별로 설명합니다. 에이전트를 사용하는 경우 브라우저 기반 지침과 함께 CLI 지침을 제공하므로 이 문서를 참조할 수 있습니다.