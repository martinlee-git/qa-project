# GitHub CI를 Hugging Face 작업으로 마이그레이션
- Source: Hugging Face Blog
- Category: ai_news
- Original URL: https://huggingface.co/blog/github-ci-hf-jobs
- Published At: Tue, 09 Jun 2026 00:00:00 GMT
- Collected At: 2026-06-11T21:49:45.537Z
- Notion Page: https://app.notion.com/p/Hugging-Face-Blog-GitHub-CI-Hugging-Face-37afc93aec57813da91ef81440e769b4
- Original Title: Migrating Your GitHub CI to Hugging Face Jobs
## Summary
우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다. 허깅페이스 채용이란? The architecture Step 1: Duplicate the dispatcher Space Step 2: Create and install the GitHub App Web setup Agent-assisted setup Step 3: Final dispatcher settings runs-on</code>"> Step 4: Change runs-on Step 5: Test it out Results If you have a GitHub repository and you have GitHub Actions enabled, you probably use GitHub-hosted runners for CI. That is the default for many projects because it is simple: add a workflow, write runs-on: ubuntu-latest , GitHub는 머신을 제공합니다. 이 기본값은 편리하지만 GitHub Actions는 속도가 느릴 수도 있습니다.

## Original Description

We’re on a journey to advance and democratize artificial intelligence through open source and open science.
## Key Points
- 우리는 오픈 소스와 오픈 사이언스를 통해 인공 지능을 발전시키고 민주화하기 위한 여정을 진행하고 있습니다.
- 허깅페이스 채용이란?
- 아키텍처 1단계: 디스패처 공간 복제 2단계: GitHub 앱 웹 설정 생성 및 설치 에이전트 지원 설정 3단계: 최종 디스패처 설정 실행</code>"> 4단계: 실행 변경 5단계: 테스트 결과 GitHub 저장소가 있고 GitHub Actions가 활성화된 경우 CI용 GitHub 호스팅 실행기를 사용할 가능성이 높습니다.
## Excerpt
허깅페이스 채용이란? The architecture Step 1: Duplicate the dispatcher Space Step 2: Create and install the GitHub App Web setup Agent-assisted setup Step 3: Final dispatcher settings runs-on</code>"> Step 4: Change runs-on Step 5: Test it out Results If you have a GitHub repository and you have GitHub Actions enabled, you probably use GitHub-hosted runners for CI. That is the default for many projects because it is simple: add a workflow, write runs-on: ubuntu-latest , and GitHub gives you a machine. That default is convenient, but it also has limits. GitHub Actions can be slow or down for maintenance, the hosted machines are generic, and GPU access is not something most open-source projects can just turn on. For Trackio , those limits started to matter. We wanted both reliable CPU CI for basic unit tests and frontend checks, but also GPU CI for tests that need to run on actual CUDA hardware. So built an alternative: keep GitHub Actions in charge of CI, but run the jobs on Hugging Face Jobs . The result: Trackio's CI now runs on Hugging Face Jobs and streams back real-time logs, cutting our CI time for CPU jobs by about 30% and enabling a whole new test suite that runs on GPU machines ! In this article, we explain step-by-step how to recreate the same setup for your GitHub repo. If you are using an agent, you can point it to this article, since we provide CLI instructions alongside browser-based instructions for us humans.