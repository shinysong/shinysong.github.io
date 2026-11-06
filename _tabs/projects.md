---
layout: page
title: Projects
permalink: /projects/
icon: fas fa-layer-group
order: 1
---

연구 및 개발 프로젝트 목록입니다.

## 1. 데이터맵·주소 지식그래프 및 LLM 검색 프로젝트

| 프로젝트 | 핵심 내용 | 기술 및 키워드 |
|---|---|---|
| **Shannon (LLM을 활용한 데이터 검색)** | 지식그래프와 검색 엔진, LLM을 결합한 데이터셋 탐색·검색 시스템 | `Knowledge Graph`, `Elasticsearch`, `Django`, `Vue.js`, `LLM` |
| **데이터맵 표준** | 공공·민간 데이터 카탈로그 상호운용을 위한 데이터맵 어휘 및 가이드라인 표준 설계 | `Standard`, `Ontology`, `Knowledge Graph` |
| **데이터맵 검색** | 온톨로지 기반 데이터 카탈로그 통합 검색 서비스 | `Ontology`, `Knowledge Graph`, `Elasticsearch`, `Vue.js`, `Django` |
| **데이터맵 대시보드** | 기관별·분야별 데이터 개방 및 연결 현황 시각화 대시보드 | `Ontology`, `Knowledge Graph`, `Django` |
| **기관 주소를 활용한 Wikidata 연계** | 공공기관 주소 지식모델과 Wikidata 개체를 연결하고 3차원 그래프로 시각화 | `Ontology`, `Knowledge Graph`, `Wikidata`, `3D-force-graph` |
| **Entity Search** | 주소 및 기관 개체 식별·연계 검색 도구 | `Ontology`, `Address` |

---

## 2. SHACL-GraphRAG 및 규칙 생명주기 연구 (2026)

기업·산업 데이터(제조 공정, 금융 GLEIF 법인 관계, YAGO 지식 그래프, BPI 2019 구매 로그)에서 명시적 제약 계층(SHACL·동일 정책 Python 규칙)과 하이브리드 GraphRAG가 의사결정 지원 및 감사(audit) 정확도에 미치는 영향을 단계별로 측정한 연구입니다.

- **사용 기술**: Python (`uv`), RDFLib, pySHACL, Neo4j (Cypher), FAISS, OpenRouter

| 단계 | 연구 질문 | 구현 메커니즘 | 주요 확인 내용 |
|---|---|---|---|
| **Stage A: 규칙 채택 게이트** | 자동 추출한 규칙이 정상 데이터를 오차단하지 않는가 | 양성·음성 반례 대조(`CEM`) 기반 채택·기각 게이트 | 합성·실데이터 벤치마크에서 부적격 규칙 사전 차단 |
| **Stage B: 표적 재조회** | 검색 누락과 원천 데이터 결함을 어떻게 구분하는가 | SHACL 위반 포커스 노드·경로만 좁혀 원천 재조회 | 전체 그래프 재탐색 없이 누락 근거 복구 |
| **Stage C: 무조인 규칙 진화** | 예외 조건이 추가될 때 애플리케이션 코드를 고쳐야 하는가 | 파이썬 조인 코드 수정 없이 선언적 Shape만 교체 | 조인 코드 변경 0줄로 정책 변경 대응 |
| **Stage D: 사후 검토** | 초안 답변 생성 후 검증 보고서를 주면 오류가 수정되는가 | 6개 모델 대상 동일 초안 대비 자체 검토 vs 구조화 보고서 비교 | 단일 목표 및 복합 산술·승인 문항에서의 수정·보류 행동 분석 |
