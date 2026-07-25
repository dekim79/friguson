---
layout: page
lang: ko
title: Workbench
subtitle: 작업대 — 진행 중이거나 완성한 제작물의 기록입니다.
permalink: /workbench/
alt_url: /en/workbench/
description: "㈜프리거슨이 설계·제작하고 있는 고열유속 냉각 시스템과 커스텀 프로젝트의 작업 기록, Workbench입니다."
---

<section style="padding-top:0;">
  <div class="eyebrow">Workbench</div>
  <h2>만들고 있는 것, 이미 만든 것</h2>
  <p>Workbench는 프리거슨이 의뢰받아 풀었거나, 자체적으로 진행 중인 제작물의 기록입니다. 설명보다 결과로 남깁니다.</p>
</section>

<section class="soft log-entry">
  <div class="log-head">
    <span class="status-pill status-ongoing">진행중</span>
    <div class="eyebrow" style="margin:0;">Flagship Project</div>
  </div>
  <h2>D2C 초고열유속 냉각 시스템</h2>
  <p>발열 칩셋에 가장 가까운 지점에서 직접 열을 제거하는 Direct-to-Chip(D2C) 시스템. 상변화 열전달을 이용해, 다수의 장비를 개별 공랭으로 식히는 방식보다 훨씬 높은 열유속을 안정적으로 처리합니다. 4가지 요소기술로 나눠 진행 중입니다.</p>

  <div class="grid grid-2" style="margin-top:24px;">
    <div class="card">
      <h3>1. Cold Plate 설계 및 제조</h3>
      <p>마이크로채널 기반 유로 구조와 재질을 최적 설계하여, 고발열 칩셋에 직접 장착되는 방열 핵심 부품을 제작합니다.</p>
    </div>
    <div class="card">
      <h3>2. CDU (Coolant Distribution Unit)</h3>
      <p>펌프, 열교환기, 수질정화필터, 제어로직을 컴팩트하게 통합한 냉각수 분배 장치를 설계·제작합니다.</p>
    </div>
    <div class="card">
      <h3>3. 최종 열교환기 및 시스템 설계</h3>
      <p>공냉/수냉 방식의 최종 열교환기를 선정하고, 전체 냉각 루프를 하나의 시스템으로 통합 설계합니다.</p>
    </div>
    <div class="card">
      <h3>4. 센서 및 제어시스템</h3>
      <p>열전대 및 DAQ 기반 정밀 온도 측정과 유량·압력 제어를 통해 운용 안정성과 균일한 냉각 성능을 확보합니다.</p>
    </div>
  </div>

  <figure class="figure" style="margin-top:32px;">
    <img src="{{ '/assets/images/diagram-d2c-system.png' | relative_url }}" alt="D2C 통합 시스템 개념도: 고성능 Cold Plate, CDU, 최종 열교환기 연결 구조">
    <figcaption>D2C 통합 시스템 개념도 — Cold Plate ↔ CDU ↔ 최종 열교환기 (실측 사진·IR 열화상으로 교체 예정)</figcaption>
  </figure>

  <figure class="figure" style="margin-top:20px;">
    <img src="{{ '/assets/images/diagram-rd-roadmap.png' | relative_url }}" alt="5단계 R&D 로드맵: 이론적 분석, Cold Plate 설계, 시작품 제작, 성능 실험, 종합 평가">
    <figcaption>1단계 이론적 분석 → 2단계 Cold Plate 최적 설계 → 3단계 시작품 제작 → 4단계 성능 실험 및 검증 → 5단계 종합 평가 및 상용화 검증</figcaption>
  </figure>

  <ul class="badge-list" style="margin-top:24px;">
    <li class="badge">AI·데이터센터</li>
    <li class="badge">전력반도체</li>
    <li class="badge">미래차 전장 시스템</li>
    <li class="badge">PUE 1.1 목표</li>
  </ul>

  <a class="btn btn-primary" href="{{ '/toolshop/' | relative_url }}" style="margin-top:8px;">완성된 부품은 Toolshop에서 →</a>
</section>

<section>
  <div class="eyebrow">Next</div>
  <h2>다음 기록</h2>
  <div class="grid grid-2">
    <div class="card log-placeholder">
      <span class="status-pill status-soon">기록 준비 중</span>
      <h3>다음 작업 기록</h3>
      <p class="text-soft">새로운 제작 기록이 계속 추가됩니다.</p>
    </div>
    <div class="card log-placeholder">
      <span class="status-pill status-soon">기록 준비 중</span>
      <h3>다음 작업 기록</h3>
      <p class="text-soft">새로운 제작 기록이 계속 추가됩니다.</p>
    </div>
  </div>
</section>

<section class="soft" style="text-align:center;">
  <h2>당신의 프로젝트도 이 작업대 위에 올라올 수 있습니다</h2>
  <p class="text-soft">기성품으로 나오지 않는, 나오기 힘든 무언가를 만들고 싶다면 Workshop에서 함께 설계합니다.</p>
  <a class="btn btn-primary" href="{{ '/workshop/' | relative_url }}">제작 의뢰하기</a>
</section>
