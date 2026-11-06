---
layout: page
title: 프로젝트
permalink: /projects/
icon: fas fa-layer-group
order: 1
---

연구 질문에서 출발해 데이터 파이프라인·검증 엔진·정량 평가까지 직접 설계하고 구현한 프로젝트들을 정리합니다.

<div class="project-grid">
  <div class="project-card">
    <div class="bento-badge-row">
      <span class="bento-tag">FLAGSHIP · 2026</span>
      <span class="bento-meta">Python · RDFLib · pySHACL · Neo4j</span>
    </div>
    <h3>SHACL-GraphRAG &amp; 규칙 생명주기 실험실</h3>
    <p>
      기업·산업 데이터(제조 공정, 금융 GLEIF 법인 관계, YAGO 지식 그래프, BPI 2019 구매 로그)에서 명시적 제약 계층(SHACL/Python 규칙)과 하이브리드 GraphRAG가 의사결정 지원 및 감사(audit) 정확도에 미치는 영향을 단계별로 측정한 연구 프로젝트입니다.
    </p>
    <div class="bento-actions" style="margin-top: 0.9rem;">
      <a href="https://shinysong.github.io/shacl-graphrag/" class="bento-btn primary">문서 사이트</a>
      <a href="https://shinysong.github.io/shacl-graphrag/experiments/actionable-evidence-demo/" class="bento-btn">라이브 데모</a>
      <a href="https://shinysong.github.io/shacl-graphrag/experiments/seminar/seminar.pdf" class="bento-btn">25p 세미나 PDF</a>
      <a href="https://github.com/shinysong/shacl-graphrag" class="bento-btn"><i class="fab fa-github"></i> 코드</a>
    </div>
    <div class="project-badges">
      <span class="project-badge">SHACL ValidationReport</span>
      <span class="project-badge">Neo4j Cypher + Dense Vector</span>
      <span class="project-badge">Post-Answer Review</span>
    </div>
  </div>

  <div class="project-card">
    <div class="bento-badge-row">
      <span class="bento-tag accent">ARCHIVE · 2026</span>
      <span class="bento-meta">18 Deep-Dive Reviews</span>
    </div>
    <h3>지식 그래프 · GraphRAG · 제조 추적성 문헌 아카이브</h3>
    <p>
      학술 논문과 오픈소스 도구를 요약하는 데 그치지 않고, 원문의 수식·도면·코호트 분모·재현성 조건을 챕터별로 대조해 정리한 기술 리뷰 시리즈입니다.
    </p>
    <div class="bento-actions" style="margin-top: 0.9rem;">
      <a href="/categories/" class="bento-btn primary">주제별 분류 보기</a>
      <a href="/posts/review-rdf2pg/" class="bento-btn">rdf2pg 심층 리뷰</a>
      <a href="/posts/review-clinical-ontology-rag/" class="bento-btn">의료 온톨로지 RAG 리뷰</a>
    </div>
    <div class="project-badges">
      <span class="project-badge">GraphRAG-Bench</span>
      <span class="project-badge">OWL &amp; SHACL Semantics</span>
      <span class="project-badge">Battery &amp; EV Traceability</span>
    </div>
  </div>
</div>

## 대표 연구 아키텍처 요약 (`shacl-graphrag`)

| 단계 | 핵심 질문 | 구현 메커니즘 | 주요 검증 결과 |
|---|---|---|---|
| **Stage A — 규칙 채택 게이트** | 자동 추출한 규칙이 정상 데이터를 오차단하지 않는가? | 양성/음성 반례 대조(`CEM`) 기반 채택·기각 게이트 | 합성·실데이터 벤치마크에서 부적격 규칙 사전 차단 |
| **Stage B — 표적 재조회** | 검색 누락과 원천 데이터 결함을 어떻게 구분하는가? | SHACL 위반 포커스 노드·경로만 좁혀 원천 재조회 | 전체 그래프 재탐색 없이 누락 근거 복구 |
| **Stage C — 무조인 규칙 진화** | 예외 조건이 추가될 때 애플리케이션 코드를 고쳐야 하는가? | 파이썬 조인 코드 수정 없이 선언적 Shape만 교체 | 조인 코드 변경 0줄로 정책 변경 대응 |
| **Stage D — 사후 검토(Post-Answer Review)** | 초안 답변 생성 후 검증 보고서를 주면 오류가 수정되는가? | 6개 모델 대상 동일 초안 대비 자체 검토 vs 구조화 보고서 비교 | 단일 목표 및 복합 산술·승인 문항에서의 수정/보류 행동 분석 |
