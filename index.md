---
layout: home
lang: ko
title: "프리거슨 | FRIGUSON — 고열유속 냉각 공작소"
description: "㈜프리거슨은 상변화 열전달 기반 Direct-to-Chip(D2C) 냉각 시스템을 설계·제작하고, 대학·기업 연구소를 위한 실험장치를 만드는 냉각 공작소입니다."
permalink: /
alt_url: /en/
hero_tagline: "General Purpose Technology for Cooling"
hero_title: "고열유속을, 발생하는 그 자리에서 없앱니다."
hero_lead: "상변화 열전달 기반 Direct-to-Chip(D2C) 시스템으로 초고집적 GPU·전력반도체의 발열 한계를 다시 설계하는 냉각 공작소, 프리거슨입니다."
hero_primary_label: "작업대 보기"
hero_primary_url: /workbench/
hero_secondary_label: "제작 의뢰하기"
hero_secondary_url: /workshop/
hero_image: /assets/images/diagram-d2c-system.png
hero_image_alt: "D2C 냉각 시스템 개념도 — Cold Plate, CDU, 최종 열교환기"
hero_image_caption: "Cold Plate가 칩 표면에서 직접 열을 흡수합니다. (실측 사진·IR 열화상으로 순차 교체 예정)"
---

<section>
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">The Workshop</div>
      <h2>공작소를 둘러보세요</h2>
      <p class="text-soft">기성품으로 나오지 않는, 나오기 힘든 무언가를 만들고 싶을 때 방문하는 공간입니다.</p>
    </div>
    <div class="grid grid-4">
      <div class="card">
        <h3>Workbench</h3>
        <p>작업대. 진행 중이거나 완성한 제작물의 기록입니다.</p>
        <a class="card-link" href="{{ '/workbench/' | relative_url }}">작업대 보기 →</a>
      </div>
      <div class="card">
        <h3>Toolshop</h3>
        <p>도구함. 이미 완성해 정가로 판매하는 부품·장비.</p>
        <a class="card-link" href="{{ '/toolshop/' | relative_url }}">도구함 보기 →</a>
      </div>
      <div class="card">
        <h3>Workshop</h3>
        <p>작업실. 세상에 없는 실험장치를 함께 설계·제작합니다.</p>
        <a class="card-link" href="{{ '/workshop/' | relative_url }}">제작 의뢰하기 →</a>
      </div>
      <div class="card">
        <h3>Archive</h3>
        <p>서재. 실험기법과 계측장비 노하우를 기록합니다.</p>
        <a class="card-link" href="{{ '/experimental-world/' | relative_url }}">서재 보기 →</a>
      </div>
    </div>
  </div>
</section>

<section class="soft">
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">From the Workbench</div>
      <h2>지금 만들고 있는 것</h2>
    </div>
    <div class="grid grid-2" style="align-items:center;">
      <figure class="figure">
        <img src="{{ '/assets/images/diagram-rd-roadmap.png' | relative_url }}" alt="5단계 R&D 로드맵">
        <figcaption>1단계 이론적 분석 → 5단계 종합 평가 및 상용화 검증</figcaption>
      </figure>
      <div>
        <span class="status-pill status-ongoing">진행중</span>
        <h3 style="margin-top:14px;">D2C 초고열유속 냉각 시스템</h3>
        <p>Cold Plate, CDU, 최종 열교환기, 센서·제어 — 4가지 요소기술로 나눠 상용화 수준까지 밀어붙이고 있습니다.</p>
        <a class="btn btn-outline" href="{{ '/workbench/' | relative_url }}">작업대에서 전체 기록 보기</a>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">Track Record</div>
      <h2>숫자로 남은 것</h2>
    </div>
    <div class="stat-row">
      <div class="stat"><span class="num">20+</span><span class="label">대표이사 열유체공학 연구 경력(년)</span></div>
      <div class="stat"><span class="num">40+</span><span class="label">국제학술지(SCI) 논문</span></div>
      <div class="stat"><span class="num">Top 2%</span><span class="label">World Top 2% Scientist 선정</span></div>
      <div class="stat"><span class="num">PUE 1.1</span><span class="label">목표 시스템 에너지효율지표</span></div>
    </div>
  </div>
</section>

{% assign latest = site.experiments_ko | sort: "date" | reverse %}
{% if latest.size > 0 %}
<section class="soft">
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">Archive</div>
      <h2>서재의 최근 기록</h2>
      <p class="text-soft">실험기법과 계측장비에 대한 최신 글을 확인해보세요.</p>
    </div>
    <div class="article-grid">
      {% for post in latest limit: 3 %}
      <a class="article-card" href="{{ post.url | relative_url }}">
        <div class="thumb">
          {% if post.image %}<img src="{{ post.image | relative_url }}" alt="{{ post.title }}">{% else %}🧪{% endif %}
        </div>
        <div class="body">
          <div class="cat">{{ post.category }}</div>
          <h3>{{ post.title }}</h3>
          <p class="excerpt">{{ post.excerpt }}</p>
          <div class="meta">{{ post.date | date: "%Y.%m.%d" }}</div>
        </div>
      </a>
      {% endfor %}
    </div>
  </div>
</section>
{% endif %}

<section>
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">Toolshop</div>
      <h2>도구함 미리보기</h2>
    </div>
    <div class="grid grid-3">
      <div class="card shop-card">
        <div class="shop-thumb">사진 준비 중</div>
        <h3>D2C Cold Plate 모듈</h3>
        <div class="shop-price">가격 문의</div>
      </div>
      <div class="card shop-card">
        <div class="shop-thumb">사진 준비 중</div>
        <h3>컴팩트 CDU</h3>
        <div class="shop-price">가격 문의</div>
      </div>
      <div class="card shop-card">
        <div class="shop-thumb">사진 준비 중</div>
        <h3>D2C 통합 패키지</h3>
        <div class="shop-price">가격 문의</div>
      </div>
    </div>
    <div style="text-align:center; margin-top:32px;">
      <a class="btn btn-outline" href="{{ '/toolshop/' | relative_url }}">도구함 전체 보기</a>
    </div>
  </div>
</section>

<section class="soft">
  <div class="container" style="text-align:center;">
    <h2>세상에 없는 무언가를 만들고 싶으신가요?</h2>
    <p class="text-soft">설계, 제작, 이론, 학문적 디스커션까지 — 아이디어 단계부터 함께 만듭니다.</p>
    <a class="btn btn-primary" href="{{ '/workshop/' | relative_url }}">제작 의뢰하기</a>
  </div>
</section>
