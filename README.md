  # 👋 이래영 · QA Engineer
  효율을 설계하는 4년차 QA. 자동화 스크립트와 테스트 전략으로 **신뢰 가능한 배포**를 만듭니다.

  ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
  ![Selenium](https://img.shields.io/badge/Selenium-43B02A?logo=selenium&logoColor=white)
  ![Postman](https://img.shields.io/badge/Postman-FF6C37?logo=postman&logoColor=white)
  ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)
  ![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)
  ![Jira](https://img.shields.io/badge/Jira-0052CC?logo=jira&logoColor=white)
  ![Notion](https://img.shields.io/badge/Notion-000000?logo=notion&logoColor=white)
  ![Obsidian](https://img.shields.io/badge/Obsidian-7c3aed?logo=obsidian&logoColor=white)
  ![Claude_Code](https://img.shields.io/badge/Claude_Code-D97757?logo=anthropic&logoColor=white)
  ![MCP](https://img.shields.io/badge/MCP-000000?logo=anthropic&logoColor=white)

  ---

  ##  About My Work
  - 빠른 배포 주기에서도 **위험도가 높은 부분을 먼저 확인**하는 QA 전략을 세웁니다.
  - 내가 하는 일의 목적을 알고, 동료들과의 협업을 중요시 합니다.
  - 테스트 결과와 회고를 기록해 두어, 팀이 다음 배포에서 더 나은 결정을 할 수 있도록 돕습니다.
  - Firebase 이벤트 로그나 DB 데이터를 활용해 **문제의 원인과 흐름**을 추적하는 걸 좋아합니다.

  ---
  ## 📄 Experience (요약)
  - **퀸잇(라포랩스)**: App/WebView/Admin 정기 배포 QA, 케이스 표준화, 핫픽스 회고 체계 → *리뷰 속도 ~30% 단축, 핫픽스 ~50% 감소*
  - **디케이테크인**: 메시징 백업/프로모션 QA(UX+API+DB 통합) → *오픈 첫 주 CS 0건*
  - **어니컴**: 반복 테스트 자동화 PoC → *TC 40% 자동화, 이슈 검출률 2배*

  ---
  ##  Tech Stack
  - **테스트 설계** · 경계값 · 동등분할 · Pairwise · 상태 전이 · 탐색적 테스트
  - **자동화** · Python · Selenium(POM) · Pytest
  - **API 검증** · Postman · REST API · JSON Schema Validation
  - **관찰/분석** · Firebase · Chrome DevTools · MySQL
  - **협업** · Jira ·  Notion · Confluence · Slack
  - **지식 관리 · AI 활용** · Obsidian · Claude Code · MCP (Jira · Slack 자동 동기화)
  ---

  ## 📑 Projects (개인 프로젝트)
  ### 1) Musinsa PDP **AI 추천** 역기획 QA
  > ⚠️ 해당 프로젝트는 **개인 연구**이며, 해당 기업과 **아무런 관계가 없습니다.**>

  #### 📌 프로젝트 개요
  - **목적**: 상용화된 무신사 상품 상세 페이지(PDP)의 **AI 추천 기능**을 실제 사용자 관점에서 분석하고
    서비스의 기획 의도와 품질 리스크를 역으로 추론하고 테스트 전략을 세우기 위한 목적입니다.
  - **핵심 포인트**
    - 단순히 화면을 보는 수준이 아니라, 추천 API 응답과 UI 매칭을 분석
    - 테스트 설계 기법(경계값분석 등)을 실제 시나리오에 적용
    - 실무에서 작성하는 QA 문서 흐름(리뷰 → 전략 → 시나리오/케이스) 그대로 재현

  ### 📑 산출물
  1. [역기획 리뷰](./docs/01_reverse_review.pdf)
     - 상용화된 기능을 사용자 관점에서 분석하고 기획 의도를 추론한 문서입니다.
  2. [테스트 전략 수립](./docs/02_test_strategy.md)
     - 리스크 기반 접근법을 통해 **무엇을 우선 검증할 것인가**를 정의했습니다.
  3. [테스트 시나리오 & 케이스 도출 (Markdown)](./docs/03_test_scenario_cases.md)
      - 주요 사용자 시나리오를 도출하고, 상세 테스트 케이스를 설계했습니다.
     - 사용자 흐름 중심의 시나리오와 세부 테스트 케이스 입니다.
     - 🔗 [상세 테스트 케이스 (Google
  Sheet)](https://docs.google.com/spreadsheets/d/1WE2UYtZpcLHk2i0Uj8kEk94Liuszb_SI9imxK_xY2z4/edit?gid=1025142518#gid=1025142518)

  ---

  ### 2) QA Knowledge Vault — Obsidian × Claude Code 기반 지식 관리 시스템

  #### 📌 프로젝트 개요
  - **목적**: 휘발되는 QA 경험을 **재사용 가능한 자산으로 누적**하기 위한 개인용 LLM 기반 지식 관리 시스템 구축
  - **문제 인식**
    - AI 시대 정보 과부하 → 한 명이 받아내고 기억하는 데 한계
    - 노션·컨플루언스 같은 공식 문서는 팀 정렬용 → 개인 회상으로 직접 변환되지 않음
    - 빠른 배포 사이클에서 ISTQB의 **경험기반 테스팅(Experience-based Testing)** 자산화 어려움
  - **해결 방향**
    - Obsidian vault에 모든 결정·이슈·정책을 박제 (append-only · markdown-first)
    - Claude Code 슬래시 스킬이 자동 분류·연결·재사용 수행
    - PARA 변형 폴더 구조 + 도메인 MOC(Map of Content) 기반 양방향 백링크

  #### 📈 운영 성과 (active iteration 중)
  - 📑 **인사이트 12건** 원자 단위로 누적 → 다음 프로젝트 부트스트랩 시 자동 컨텍스트 로드
  - 📜 **운영 정책 4건** · **이슈 히스토리 3건** · **완료 프로젝트 3건** · **도메인 MOC 3건**
  - ⚡ **슬래시 스킬 약 10개** 로 반복 분류 결정 자동화 (`/new-project` · `/close-project` · `/inbox-cleanup` 등)
  - 🔍 **슬랙 65개 메시지 스레드** 에서 **미기록 결정 2건 자동 발견** → 결정 로그 D12·D13 시간순 append
  - 🛡️ **AI 자동 작성 시스템의 가드레일 4규칙** 박제 → "그럴듯한 추측이 사실처럼 박제되는" 위험 차단

  #### 📑 산출물
  - 🔗 [GitHub Repository — qa-knowledge-vault](https://github.com/raeyoung-works/qa-knowledge-vault)
  - 🔗 발표 자료 · 회고 블로그 글 (추후 공개 예정)

  ---

  ## 📣 External Activity
  ####  [QA Korea Conference 발표](https://www.linkedin.com/posts/qa-korea-conference_qa-softwareqa-testing-activity-7346731415339716608-Qubp)
  - 📅 **2025.07 — QA Korea Conference 연사**
  - **발표 주제**: QA 커리어 성장 인사이트: 회고와 목표 세분화
  - **발표 내용 요약**
    - 커리어 성장 과정에서 겪은 고민과 인사이트 공유
    - 4L 회고 기반 자기 성찰과 실천 사례
    - 목표를 일을 작은 단계로 나누어 실현하는 방법론 제안

  ### ✍️ Blog : QA 기록집
  - [QA의 Lunch & Learn 문화 도입 후기](https://rae-gi.tistory.com/115)
  - [QA 포트폴리오 인사이트 공유](https://rae-gi.tistory.com/134)
  - [기술용어들을 정리하는 한줄용어](https://rae-gi.tistory.com/category/%E2%9C%8F%EF%B8%8F%20%ED%95%9C%EC%A4%84%20%EC%9A%A9%EC%96%B4)
  > 📌 블로그 전체 보러가기: [https://rae-gi.tistory.com](https://rae-gi.tistory.com)


  ---


  ## 📬 Contact
  - Email: raeyoung.works@gmil.com
  - Blog: https://rae-gi.tistory.com
  - LinkedIn: https://www.linkedin.com/in/raeyoung-lee
