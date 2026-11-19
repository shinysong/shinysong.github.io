---
layout: page
title: Reviews
permalink: /reviews/
icon: fas fa-book-open
order: 2
---

지식 그래프, GraphRAG, SHACL(SHACL 1.2 포함), 속성 그래프 표준(PG-Keys·PG-Schema), 제조 추적성과 관련된 논문 및 표준·오픈소스 도구를 분석한 리뷰 목록입니다. 주제별로는 [카테고리](/categories/) 또는 [태그](/tags/)에서 모아 볼 수 있습니다.

## 장별 심층 리뷰 (원문 도면·수식·표준 명세 대조, 12편)

- **[W3C SHACL 1.2 리뷰: 2017년 SHACL 1.0에서 RDF 1.2·규칙 추론·에이전트 메타데이터까지의 진화](/posts/review-shacl-12/)** (2026.11.19)  
  W3C SHACL 1.2 Overview 및 SHACL 1.2 Core 명세 분석. 2017년 오리지널 SHACL(1.0)과 SHACL-AF의 배경·한계부터 9개 모듈형 명세 패밀리 재편, RDF 1.2 Reification 검증(`sh:reifierShape`), `sh:ShapeClass`, `sh:targetWhere`, `sh:uniqueValuesFor`, `sh:closed sh:ByTypes`, 불완전 데이터(`sh:incomplete`), LLM 에이전트·코드 생성 어노테이션(`sh:intent`, `sh:agentInstruction`, `sh:unit`) 및 1.0 vs. 1.2 전수 비교
- **[PG-Schema 리뷰: 다중 상속 타입(PG-Types)과 PG-Keys를 결합한 속성 그래프 스키마 표준 청사진](/posts/review-pg-schema/)** (2026.11.19)  
  ACM SIGMOD 2023 논문 분석. 금융 사기 그래프 스키마 예제, `STRICT`·`LOOSE`·`OPEN` 3계층 개방성 제어와 다중 상속(`&`) 형식 의미론($\oplus$), PG-Keys 통합 제약, SHACL·OWL·상용 그래프 DB 등 21개 스키마 체계의 16개 기능 전수 비교
- **[PG-Keys 리뷰: 속성 그래프의 노드·간선·속성에 일관되게 적용하는 키와 무결성 제약](/posts/review-pg-keys/)** (2026.11.19)  
  ACM SIGMOD 2021 논문 분석. `EXCLUSIVE`·`MANDATORY`·`SINGLETON` 조합으로 정의되는 4대 키 계층, 질의 기반 범위(Scope)와 이웃 위상 서술자(Descriptor), 조건 (K1)–(K3)의 Cypher 검증 질의 재작성 및 SHACL·OWL(`owl:hasKey`) 비교
- **[그래프 DB와 온톨로지 추론기 비교: Amazon Neptune, Neo4j n10s, RETE·Hypertableau부터 최신 도구까지](/posts/review-neptune-reasoners-rete-hypertableau/)** (2026.11.06)  
  Amazon Neptune·Virtuoso·Blazegraph·GraphDB·Neo4j(n10s) 비교, 추론기와 SHACL 검증의 역할 분담, Forgy(1982) RETE·Motik 외(2009) Hypertableau 원 논문 알고리즘 및 HermiT 코드 구조, 2026년 오픈소스 생태계와 비교 실험 설계 종합 정리
- **[의료 온톨로지 RAG 리뷰: Neo4j와 n10s를 이용한 검색·분류 실험](/posts/review-clinical-ontology-rag/)** (2026.11.05)  
  MIMIC-IV 패혈증 분류 실험과 생성 전 의미 필터(`O(C_h)`), 표 1·표 2의 평가 분모 및 ROC 곡선 형태를 장별로 대조한 분석
- **[RAG vs. GraphRAG 리뷰: 상세 질문·관계 질문·답 없는 질문의 차이](/posts/review-rag-vs-graphrag/)** (2026.11.05)  
  NQ·HotpotQA·MultiHop-RAG·NovelQA·요약 과제에서 7개 RAG/GraphRAG 변형 비교, 추론 전략(Vanilla·Rerank·IRCoT), 정오답 혼동 행렬, Selection/Integration 결합 비용과 Null 질문 취약성 분석
- **[GraphRAG-Bench 리뷰: 질문 난도와 검색·생성 비용을 나눠 보는 평가](/posts/review-when-graphs-rag/)** (2026.11.05)  
  ICLR 2026 GraphRAG-Bench의 Level 1–4 질문 난도 체계, Novel·Medical 코퍼스에서의 생성·검색(Evidence Recall vs. Context Relevance)·그래프 위상·질의당 토큰 비용을 장별로 대조한 분석
- **[rdf2pg 리뷰: 같은 지식 그래프를 RDF와 속성 그래프로 조회하기](/posts/review-rdf2pg/)** (2026.11.05)  
  도메인별 SPARQL 매핑을 통한 RDF→LPG 변환 구조, 4개 그래프 DB 질의 성능 벤치마크, 의미·정보 보존 조건 분석
- **[OWL과 SHACL 의미론 리뷰: 추론한 그래프를 무엇으로 검증할 것인가](/posts/review-owl-shacl-semantics/)** (2026.11.05)  
  *Artificial Intelligence* (2026) 게재 논문 분석. $\text{Horn-}\mathcal{ALCHIQ}$ 온톨로지와 SHACL 결합 시 Core Universal Model(엄격한 정준 모델) 의미론, 무한 익명 트리를 피하는 Stratified SHACL 재작성 알고리즘과 복잡도(ExpTime / PTime) 정리
- **[PolicyKG 리뷰: 정책 문장의 의무·허용·금지를 SHACL로 옮기기](/posts/review-policykg/)** (2026.11.05)  
  4단계 LangGraph 파이프라인, NL→FOL+Deontic→SHACL 결정론적 컴파일 추적, 3요소 Corpus Adapter를 통한 어휘 정렬, 443/351/69 분모별 평가와 오픈 모델 4종·절제 연구 6종 대조
- **[SHACL 업데이트 검증 리뷰: 데이터를 바꾸기 전에 제약 보존을 판단하기](/posts/review-shacl-updates/)** (2026.11.05)  
  ISWC 2025 채택 논문 분석. 조건부 그래프 업데이트($\alpha = (\oplus, \ominus)$)의 정적 보존 검증, 회귀(Regression) 재작성 정리, 조각별 복잡도 및 `SHACL2FOL` + Vampire 4.9 실험 결과 분석
- **[xpSHACL 리뷰: 검증 실패를 사람이 이해할 수 있는 설명으로 바꾸기](/posts/review-xpshacl/)** (2026.11.05)  
  VLDB 2025 LLM+Graph 워크숍 논문 분석. 정당화 트리·RAG 문맥·Violation KG 캐시를 결합한 설명 가능 SHACL 검증 구조, LOV 868개 온톨로지 전수 실험 분모(431개 검증·99.48% 캐시 적중)와 반복 실행 시간 분석

---

## 주제별 전체 리뷰 (22편)

### GraphRAG & Retrieval
- [의료 온톨로지 RAG 리뷰: Neo4j와 n10s를 이용한 검색·분류 실험](/posts/review-clinical-ontology-rag/) (2026.11.05)
- [RAG vs. GraphRAG 리뷰: 상세 질문·관계 질문·답 없는 질문의 차이](/posts/review-rag-vs-graphrag/) (2026.11.05)
- [GraphRAG-Bench 리뷰: 질문 난도와 검색·생성 비용을 나눠 보는 평가](/posts/review-when-graphs-rag/) (2026.11.05)

### Graph Architecture
- [PG-Schema 리뷰: 다중 상속 타입(PG-Types)과 PG-Keys를 결합한 속성 그래프 스키마 표준 청사진](/posts/review-pg-schema/) (2026.11.19)
- [PG-Keys 리뷰: 속성 그래프의 노드·간선·속성에 일관되게 적용하는 키와 무결성 제약](/posts/review-pg-keys/) (2026.11.19)
- [그래프 DB와 온톨로지 추론기 비교: Amazon Neptune, Neo4j n10s, RETE·Hypertableau부터 최신 도구까지](/posts/review-neptune-reasoners-rete-hypertableau/) (2026.11.06)
- [rdf2pg 리뷰: 같은 지식 그래프를 RDF와 속성 그래프로 조회하기](/posts/review-rdf2pg/) (2026.11.05)

### SHACL & Knowledge Graphs
- [W3C SHACL 1.2 리뷰: 2017년 SHACL 1.0에서 RDF 1.2·규칙 추론·에이전트 메타데이터까지의 진화](/posts/review-shacl-12/) (2026.11.19)
- [OWL과 SHACL 의미론 리뷰: 추론한 그래프를 무엇으로 검증할 것인가](/posts/review-owl-shacl-semantics/) (2026.11.05)
- [PolicyKG 리뷰: 정책 문장의 의무·허용·금지를 SHACL로 옮기기](/posts/review-policykg/) (2026.11.05)
- [SHACL 업데이트 검증 리뷰: 데이터를 바꾸기 전에 제약 보존을 판단하기](/posts/review-shacl-updates/) (2026.11.05)
- [xpSHACL 리뷰: 검증 실패를 사람이 이해할 수 있는 설명으로 바꾸기](/posts/review-xpshacl/) (2026.11.05)
- [NL2SHACL-Bench 리뷰: 자연어로 만든 검증 규칙을 평가하는 전체 과정](/posts/review-nl2shacl-bench/) (2026.10.16)
- [SHACL Guru 도구 리뷰: VS Code에서 규칙을 생성하고 설명받는 과정](/posts/review-shacl-guru/) (2026.10.16)
- [shacl-test 도구 리뷰: RDF 사례와 검증 보고서를 반복 검사하는 방법](/posts/review-shacl-test/) (2026.10.16)
- [Shapes from Examples 리뷰: 그래프 사례에서 검증 규칙을 학습하는 이론](/posts/review-shapes-from-examples/) (2026.10.16)

### Manufacturing & Traceability
- [Wessel 외 논문 리뷰: 배터리 전극의 식별과 생산 이력 추적](/posts/review-battery-traceability/) (2026.10.29)
- [LG마그나 협력사 요구사항 리뷰: 추적성·변경 승인·품질 기록의 연결](/posts/review-lgmagna-traceability/) (2026.10.29)
- [MetalMind 논문 리뷰: 금속 적층제조 매뉴얼에서 작업자 지원까지](/posts/review-metalmind/) (2026.10.29)
- [Meyers 외 논문 리뷰: 제조 지식을 온톨로지와 그래프로 묶는 두 가지 방법](/posts/review-meyers-manufacturing/) (2026.10.29)

### Knowledge Graph Extraction & Rule Learning
- [반도체 특허 지식그래프 논문 리뷰: 특허 문장에서 기술 개체와 관계를 뽑는 방법](/posts/review-semiconductor-patent-kg/) (2026.10.29)
- [REGAE 리뷰: 예시를 주고받으며 정규표현식을 만드는 도구](/posts/review-regae/) (2026.10.16)
