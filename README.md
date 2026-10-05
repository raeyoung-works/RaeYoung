# 이래영 · QA Engineer

효율을 설계하는 QA 4년 11개월 차. 자동화 스크립트와 테스트 전략으로 **신뢰 가능한 배포**를 만듭니다.

[![Email](https://img.shields.io/badge/Email-raeyoung.works@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:raeyoung.works@gmail.com)
[![Blog](https://img.shields.io/badge/Blog-rae--gi.tistory.com-FF5A4A?style=flat-square&logo=tistory&logoColor=white)](https://rae-gi.tistory.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-raeyoung--lee-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/raeyoung-lee)

| **62%** | **131건** | **1회** |
|:---:|:---:|:---:|
| TC 작성~수행 시간 단축<br>(QA 스킬 벤치마크) | 누적한 QA 인사이트<br>(QA Knowledge Vault) | QA Korea Conference 연사<br>(2025.07) |

---

## About My Work

- 빠른 배포 주기에서도 **위험도가 높은 부분을 먼저 확인**하는 QA 전략을 세웁니다.
- 내가 하는 일의 목적을 알고, 동료들과의 협업을 중요시 합니다.
- 테스트 결과와 회고를 기록해 두어, 팀이 다음 배포에서 더 나은 결정을 할 수 있도록 돕습니다.
- Firebase 이벤트 로그나 DB 데이터를 활용해 **문제의 원인과 흐름**을 추적하는 걸 좋아합니다.

## Featured Work

| 프로젝트 | 무엇을 증명하나 | 링크 |
|---|---|---|
| **QA 스킬 벤치마크** | AI 스킬이 QA 시간을 정말 줄이는지 숫자로 검증. 사람 3시간 42분 → AI 1시간 24분 (**62% 단축**), 심어 둔 결함 5개를 3번 모두 첫 시도에 탐지(파일럿) | [레포](https://github.com/raeyoung-works/qa-skill-benchmark) · [심화](https://github.com/raeyoung-works/qa-skill-benchmark/blob/main/docs/deep-dive.md) · [용어집](https://github.com/raeyoung-works/qa-skill-benchmark/blob/main/docs/glossary.md) |
| **QA Knowledge Vault** | 휘발되는 QA 경험을 재사용 자산으로. 인사이트 **131건**, 슬래시 스킬 **11개**, AI 자동 작성 가드레일 4규칙 | [레포](https://github.com/raeyoung-works/qa-knowledge-vault) · [시스템 개선기](https://rae-gi.tistory.com/163) |
| **무신사 PDP AI 추천 역기획 QA** | 상용 서비스를 사용자 관점에서 분석해 리스크 기반 테스트 전략과 케이스를 설계. 개인 연구이며 해당 기업과 무관 | [역기획 리뷰](./docs/01_reverse_review.pdf) · [테스트 전략](./docs/02_test_strategy.md) · [시나리오·케이스](./docs/03_test_scenario_cases.md) · [케이스 시트](https://docs.google.com/spreadsheets/d/1WE2UYtZpcLHk2i0Uj8kEk94Liuszb_SI9imxK_xY2z4/edit?gid=1025142518#gid=1025142518) |

<details>
<summary>QA 스킬 벤치마크: 개요</summary>

- **배경**: 회사의 AX 프로젝트 팀이 진행한 EYWA 프로젝트(AI를 실무에 적용해 리드타임 단축)의 **QA 트랙**. QA용 AI 스킬이 테스트케이스 작성과 수행 시간을 실제로 줄이는지, 느낌이 아니라 **숫자로** 확인하는 측정 틀(벤치마크)을 만들고 운영
- **내 역할**: 백엔드 엔지니어가 만든 측정 틀을 QA 업무에 맞게 재설계하고, QA 전용 저장소 구성·사람 실측·측정 운영·결과 분석을 주도
- **측정 방식**: 같은 기획서와 결함 5개를 심은 시험용 서버를 고정하고 스킬만 바꿔 조건마다 3번 반복. 채점은 AI의 말이 아니라 **테스트 재실행으로 확인한 실제 실패**로 하고, 채점용 목록은 AI가 볼 수 없게 격리
- **결과**: 같은 기획서 기준 소요 시간 사람 3시간 42분 → 스킬을 쓴 AI 1시간 24분(62% 단축). 측정용 과제가 1개인 **파일럿 결과**
- 개선이 오히려 느려진 사례(성능 회귀), 결함이 있는데 테스트가 통과한 사례(거짓 통과)의 원인 분석과 대응 기록

</details>

<details>
<summary>QA Knowledge Vault: 개요</summary>

- **목적**: 휘발되는 QA 경험을 **재사용 가능한 자산으로 누적**하기 위한 개인용 LLM 기반 지식 관리 시스템 구축
- **문제 인식**
  - AI 시대 정보 과부하 → 한 명이 받아내고 기억하는 데 한계
  - 노션·컨플루언스 같은 공식 문서는 팀 정렬용 → 개인 회상으로 직접 변환되지 않음
  - 빠른 배포 사이클에서 ISTQB의 **경험기반 테스팅(Experience-based Testing)** 자산화 어려움
- **해결 방향**
  - Obsidian vault에 모든 결정·이슈·정책을 박제 (append-only · markdown-first)
  - Claude Code 슬래시 스킬이 자동 분류·연결·재사용 수행
  - PARA 변형 폴더 구조 + 도메인 MOC(Map of Content) 기반 양방향 백링크
- **운영 성과 (active iteration 중)**: 인사이트 **131건** · 서비스 정책 **68건** · 이슈 히스토리 **48건** · 완료 프로젝트 **33건** · 도메인 MOC **18개** · 슬래시 스킬 **11개**(`/new-project` · `/close-project` · `/inbox-cleanup` 등)
- **가드레일**: AI 자동 작성 시스템의 가드레일 4규칙을 박제해 "그럴듯한 추측이 사실처럼 박제되는" 위험을 차단

</details>

<details>
<summary>무신사 PDP AI 추천 역기획 QA: 개요</summary>

> 해당 프로젝트는 **개인 연구**이며, 해당 기업과 **아무런 관계가 없습니다.**

- **목적**: 상용화된 무신사 상품 상세 페이지(PDP)의 **AI 추천 기능**을 실제 사용자 관점에서 분석하고, 서비스의 기획 의도와 품질 리스크를 역으로 추론해 테스트 전략을 세우기 위한 목적
- **핵심 포인트**
  - 단순히 화면을 보는 수준이 아니라, 추천 API 응답과 UI 매칭을 분석
  - 테스트 설계 기법(경계값분석 등)을 실제 시나리오에 적용
  - 실무에서 작성하는 QA 문서 흐름(리뷰 → 전략 → 시나리오/케이스) 그대로 재현

</details>

## Experience

| 회사 | 기간 | 한 일 | 성과 |
|---|---|---|---|
| **월급쟁이부자들** | 2026.01 ~ 현재 | 커뮤니티·중개 두 스쿼드 QA<br>개발본부 AX(AI Transformation) 프로젝트 참여<br>Obsidian × Claude Code 기반 QA 지식 관리 시스템 설계·운영 | tc-writer·e2e-writer로 TC 작성부터 E2E 수행까지 **62% 단축**<br>두 스쿼드 일정 준수율 **95%**, 운영 중 크리티컬 이슈 **0건**<br>핫픽스 월 평균 **3건 → 1건** |
| **퀸잇(라포랩스)** | 2023.07 ~ 2024.05 | App/WebView/Admin 정기 배포 QA, 케이스 표준화, 핫픽스 회고 체계 | 리뷰 속도 **~30% 단축**, 핫픽스 **~50% 감소** |
| **디케이테크인** | 2022.05 ~ 2023.07 | 메시징 백업/프로모션 QA (UX+API+DB 통합) | 오픈 첫 주 **CS 0건** |
| **어니컴** | 2020.04 ~ 2022.03 | 반복 테스트 자동화 PoC | TC **40% 자동화**, 이슈 검출률 **2배** |

## Toolbox

| 분류 | 기술 |
|---|---|
| 테스트 설계 | 경계값 · 동등분할 · Pairwise · 상태 전이 · 탐색적 테스트 |
| 자동화 | ![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white) Pytest · POM |
| API · 데이터 | ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black) REST API · JSON Schema · Chrome DevTools |
| AI · 지식 관리 | ![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white) ![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square&logo=anthropic&logoColor=white) ![Obsidian](https://img.shields.io/badge/Obsidian-7c3aed?style=flat-square&logo=obsidian&logoColor=white) (Jira · Slack 자동 동기화) |
| 협업 | ![Jira](https://img.shields.io/badge/Jira-0052CC?style=flat-square&logo=jira&logoColor=white) ![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white) Confluence · Slack |

## Talks & Writing

**QA Korea Conference 연사** (2025.07): [QA 커리어 성장 인사이트: 회고와 목표 세분화](https://www.linkedin.com/posts/qa-korea-conference_qa-softwareqa-testing-activity-7346731415339716608-Qubp) · 4L 회고 기반 자기 성찰과 목표를 작은 단계로 나누는 방법

**Blog: QA 기록집** ([전체 보기](https://rae-gi.tistory.com))

- [QA의 Lunch & Learn 문화 도입 후기](https://rae-gi.tistory.com/115)
- [QA 포트폴리오 인사이트 공유](https://rae-gi.tistory.com/134)
- [Claude Code가 없는 기능의 테스트케이스를 썼습니다](https://rae-gi.tistory.com/163)
- [기술용어들을 정리하는 한줄용어](https://rae-gi.tistory.com/category/%E2%9C%8F%EF%B8%8F%20%ED%95%9C%EC%A4%84%20%EC%9A%A9%EC%96%B4)

## Contact

raeyoung.works@gmail.com · [Blog](https://rae-gi.tistory.com) · [LinkedIn](https://www.linkedin.com/in/raeyoung-lee)
