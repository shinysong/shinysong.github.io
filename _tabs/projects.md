---
layout: page
title: 프로젝트
permalink: /projects/
icon: fas fa-layer-group
order: 1
---

진행 중이거나 완료된 연구 프로젝트와 주요 산출물을 정리한 목록입니다.

## 1. SHACL-GraphRAG 및 규칙 생명주기 연구 (2026.10 – 현재)

기업·산업 데이터(제조 공정, 금융 GLEIF 법인 관계, YAGO 지식 그래프, BPI 2019 구매 로그)에서 명시적 제약 계층(SHACL·동일 정책 Python 규칙)과 하이브리드 GraphRAG가 의사결정 지원 및 감사(audit) 정확도에 미치는 영향을 단계별로 측정한 프로젝트입니다.

- **문서 및 결과물**: [연구실 문서 사이트](https://shinysong.github.io/shacl-graphrag/) · [인터랙티브 데모](https://shinysong.github.io/shacl-graphrag/experiments/actionable-evidence-demo/) · [세미나 슬라이드 (25쪽 PDF)](https://shinysong.github.io/shacl-graphrag/experiments/seminar/seminar.pdf) · [GitHub 저장소](https://github.com/shinysong/shacl-graphrag)
- **사용 기술**: Python (`uv`), RDFLib, pySHACL, Neo4j (Cypher), FAISS, OpenRouter

| 단계 | 연구 질문 | 구현 메커니즘 | 주요 확인 내용 |
|---|---|---|---|
| **Stage A — 규칙 채택 게이트** | 자동 추출한 규칙이 정상 데이터를 오차단하지 않는가 | 양성·음성 반례 대조(`CEM`) 기반 채택·기각 게이트 | 합성·실데이터 벤치마크에서 부적격 규칙 사전 차단 |
| **Stage B — 표적 재조회** | 검색 누락과 원천 데이터 결함을 어떻게 구분하는가 | SHACL 위반 포커스 노드·경로만 좁혀 원천 재조회 | 전체 그래프 재탐색 없이 누락 근거 복구 |
| **Stage C — 무조인 규칙 진화** | 예외 조건이 추가될 때 애플리케이션 코드를 고쳐야 하는가 | 파이썬 조인 코드 수정 없이 선언적 Shape만 교체 | 조인 코드 변경 0줄로 정책 변경 대응 |
| **Stage D — 사후 검토** | 초안 답변 생성 후 검증 보고서를 주면 오류가 수정되는가 | 6개 모델 대상 동일 초안 대비 자체 검토 vs 구조화 보고서 비교 | 단일 목표 및 복합 산술·승인 문항에서의 수정·보류 행동 분석 |

---

## 2. 지식 그래프 · GraphRAG · 제조 추적성 문헌 리뷰 (2026.10 – 현재)

학술 논문과 오픈소스 도구를 요약하는 데 그치지 않고, 원문의 수식·도면·코호트 분모·재현성 조건을 장별로 대조해 기록하는 아카이브입니다.

- **탐색**: [주제별 분류 (`/categories/`)](/categories/) · [태그 (`/tags/`)](/tags/) · [연도별 아카이브 (`/archives/`)](/archives/)
- **장별 상세 분석 대표 글**:
  - [rdf2pg 리뷰 — 같은 지식 그래프를 RDF와 속성 그래프로 조회하기](/posts/review-rdf2pg/)
  - [의료 온톨로지 RAG 리뷰 — Neo4j와 n10s를 이용한 검색·분류 실험](/posts/review-clinical-ontology-rag/)
