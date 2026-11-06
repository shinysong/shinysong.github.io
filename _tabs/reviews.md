---
layout: page
title: Reviews
permalink: /reviews/
icon: fas fa-book-open
order: 2
---

지식 그래프, GraphRAG, SHACL, 제조 추적성과 관련된 논문 및 오픈소스 도구를 분석한 리뷰 목록입니다. 주제별로는 [카테고리](/categories/) 또는 [태그](/tags/)에서 모아 볼 수 있습니다.

## 장별 심층 리뷰 (원문 도면·수식·재현성 대조)

- **[그래프 DB와 온톨로지 추론기 비교: Amazon Neptune, Neo4j n10s, RETE·Hypertableau부터 최신 도구까지](/posts/review-neptune-reasoners-rete-hypertableau/)** (2026.11.06)  
  Amazon Neptune·Virtuoso·Blazegraph·GraphDB·Neo4j(n10s) 비교, 추론기와 SHACL 검증의 역할 분담, Forgy(1982) RETE·Motik 외(2009) Hypertableau 원 논문 알고리즘 및 HermiT 코드 구조, 2026년 오픈소스 생태계와 비교 실험 설계 종합 정리
- **[의료 온톨로지 RAG 리뷰: Neo4j와 n10s를 이용한 검색·분류 실험](/posts/review-clinical-ontology-rag/)** (2026.11.05)  
  MIMIC-IV 패혈증 분류 실험과 생성 전 의미 필터(`O(C_h)`), 표 1·표 2의 평가 분모 및 ROC 곡선 형태를 장별로 대조한 분석
- **[rdf2pg 리뷰: 같은 지식 그래프를 RDF와 속성 그래프로 조회하기](/posts/review-rdf2pg/)** (2026.11.05)  
  도메인별 SPARQL 매핑을 통한 RDF→LPG 변환 구조, 4개 그래프 DB 질의 성능 벤치마크, 의미·정보 보존 조건 분석

---

## 주제별 전체 리뷰 (19편)

### GraphRAG & Retrieval
- [의료 온톨로지 RAG 리뷰: Neo4j와 n10s를 이용한 검색·분류 실험](/posts/review-clinical-ontology-rag/) (2026.11.05)
- [RAG vs. GraphRAG 리뷰: 상세 질문·관계 질문·답 없는 질문의 차이](/posts/review-rag-vs-graphrag/) (2026.11.05)
- [GraphRAG-Bench 리뷰: 질문 난도와 검색·생성 비용을 나눠 보는 평가](/posts/review-when-graphs-rag/) (2026.11.05)

### Graph Architecture
- [그래프 DB와 온톨로지 추론기 비교: Amazon Neptune, Neo4j n10s, RETE·Hypertableau부터 최신 도구까지](/posts/review-neptune-reasoners-rete-hypertableau/) (2026.11.06)
- [rdf2pg 리뷰: 같은 지식 그래프를 RDF와 속성 그래프로 조회하기](/posts/review-rdf2pg/) (2026.11.05)

### SHACL & Knowledge Graphs
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
