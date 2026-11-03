# 이재희 | AI Agent Engineer

사용자의 요청을 이해하는 것에서 끝나지 않고,  
**RAG·Agent·Backend·Infra를 연결해 실제로 동작하는 AI 서비스**를 개발합니다.

복합 요청을 안전하게 실행하는 Multi-Agent 구조,  
검색 품질을 측정하고 개선하는 Retrieval Pipeline,  
운영 환경에서 재현 가능한 배포와 관측성에 관심이 있습니다.

- `LangGraph` 기반 Multi-Agent·Tool-use 설계
- `RAGAS`·Golden Dataset 기반 검색 및 응답 품질 평가
- `FastAPI`·`AWS`·`Docker` 기반 서비스 배포와 운영
- 서비스 기획부터 개발·검증·배포까지 수행한 팀 프로젝트 경험

<br>

## Featured Projects

### 1. 밥벌이 — Multi-Agent 식재료 관리 서비스

> 냉장고 조회부터 레시피 추천, 장보기, 일정 등록까지  
> 서로 의존하는 작업을 하나의 대화로 처리하는 AI 서비스

**Team Lead · AI Agent · Backend · Infra**

- Supervisor와 Domain Agent로 업무 책임 및 실행 정책 분리
- 독립 조회는 병렬, 의존 작업은 순차적으로 실행
- 변경 작업은 `preview → 사용자 확인 → commit` 방식으로 보호
- 13개 MCP Tool에 OAuth 2.1·Scope·멱등성 적용
- Langfuse로 Agent 선택, Tool 호출, 실패 지점을 Trace
- 200개 발화 기준 Hybrid Intent Router 정확도 **88.5%**
- 기능·단위·API·A/B·경계 조건을 포함한 **388건 테스트**
- AWS CDK·ECS Fargate·CloudFront 기반 운영 환경 구축

`LangGraph` `MCP` `FastAPI` `PostgreSQL` `Neo4j`  
`Langfuse` `React` `AWS CDK` `ECS Fargate` `GitHub Actions`

[Repository](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN27-FINAL-1Team) ·
[Live Service](https://www.bobbeori.com/)

---

### 2. 너로 정했다! LLM — Graph-guided Hybrid RAG

> 의미 검색과 관계 탐색을 결합한  
> 포켓몬 추천·분석·시뮬레이션 플랫폼

**Data Pipeline · Backend · UI/UX · Chrome Extension**

- 외부 API 데이터를 수집·정제해 PostgreSQL과 Neo4j에 적재
- PostgreSQL·pgvector 기반 의미 검색과 Neo4j 관계 탐색 결합
- 대량 데이터 렌더링 및 프론트엔드–백엔드 연결 병목 개선
- GitHub OAuth와 통계 데이터 병렬 수집 기능 구현
- AI 분석 기능을 브라우저에서 사용할 수 있는 Chrome Extension 개발
- Docker 기반 서비스 실행 환경 및 서버 구조 구성

`FastAPI` `PostgreSQL` `pgvector` `Neo4j`  
`LangGraph` `Streamlit` `Docker` `Chrome Extension`

[Repository](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN27-3rd-3TEAM)

---

### 3. HELBOTIN — RAG 기반 개인 맞춤 운동 서비스

> 서비스가 보유한 운동 데이터 안에서  
> 상담과 추천을 제공하는 개인 맞춤형 운동 서비스

**Service Planning · Frontend · Backend · Production Debugging**

- 약 920종의 운동 데이터를 활용한 RAG 상담 구조 설계
- 자연어 의미 검색과 운동 관계 탐색을 분리해 구성
- React·Django 기반 서비스 기능 구현 및 AWS 환경 배포
- 로컬에서는 정상인 SSE 응답이 운영 환경에서 지연되는 장애 분석
- `Browser → Host Nginx → Container → Backend` 요청 경로 검증
- Nginx Proxy Buffering을 원인으로 특정해 Token Streaming 정상화

`React` `Django` `pgvector` `Neo4j`  
`SSE` `Nginx` `Docker` `AWS EC2`

[Repository](https://github.com/EJ-pro/SKN27-4th-4team)

<br>

## Additional Experience

### KKBOX Churn Prevention System

고객 이탈 확률만 제공하는 데서 끝내지 않고,  
사용자별 이탈 원인과 Retention Action을 연결한 ML 서비스입니다.

- 30GB 이상의 원본 로그를 분석 가능한 데이터셋으로 전처리
- XGBoost와 Stacking 모델의 성능 및 운영 복잡도 비교
- Stacking 적용 후 False Positive **1,379건 → 1,189건**
- 예측 결과를 Action Board와 ROI 관점의 리텐션 전략으로 연결

`XGBoost` `LightGBM` `CatBoost` `Scikit-learn` `Streamlit` `MySQL`

[Repository](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN27-2nd-3TEAM)

<br>

## Tech Stack

**AI Engineering**

`Python` `LangGraph` `LangChain` `RAG` `MCP` `RAGAS` `Langfuse`

**Backend & Data**

`FastAPI` `Django` `PostgreSQL` `pgvector` `Neo4j` `MySQL`

**Infrastructure**

`AWS` `Docker` `GitHub Actions` `Nginx` `AWS CDK`

**Client**

`React` `JavaScript` `Kotlin` `Android`

<br>

## What I'm Working On

현재는 AI 시스템의 기능 추가보다  
**검색 품질, Agent 실행 안정성, 비용과 지연시간을 측정하고 개선하는 방법**을 공부하고 있습니다.

- Hybrid Retrieval과 Reranking 비교
- Agent Tool Selection 및 Task Completion 평가
- RAG Index Versioning과 회귀 테스트
- LLM Observability와 실패 Trace 분석

<br>

## Contact

- Email: developer0@gmail.com
- GitHub: [github.com/EJ-pro](https://github.com/EJ-pro)
- Portfolio: 포트폴리오 링크
