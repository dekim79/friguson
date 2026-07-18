---
layout: home
lang: ko
title: "프리거슨 | 전자장비 냉각 솔루션"
description: "㈜프리거슨은 초고집적 전자장비를 위한 고효율·저탄소 Direct-to-Chip(D2C) 냉각 솔루션을 개발하고, 대학·기업 연구소를 위한 실험장치를 설계·제작합니다."
permalink: /
alt_url: /en/
hero_tagline: "General Purpose Technology for Cooling"
hero_title: "전자장비 냉각의 새로운 기준, Direct-to-Chip 열관리 솔루션"
hero_lead: "㈜프리거슨은 초고집적 GPU 칩셋, 전력반도체, AI 서버를 위한 고효율·저탄소 냉각 시스템을 설계·제작하는 열유체공학 기반 딥테크 기업입니다."
hero_primary_label: "기술 살펴보기"
hero_primary_url: /technology/
hero_secondary_label: "실험장치 제작 문의"
hero_secondary_url: /lab-solutions/
---

<section>
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">Business</div>
      <h2>프리거슨이 하는 일</h2>
      <p class="text-soft">냉각 기술 개발 역량을 바탕으로 세 가지 사업 영역에서 가치를 만듭니다.</p>
    </div>
    <div class="grid grid-3">
      <div class="card">
        <div class="icon">❄</div>
        <h3>전자장비 냉각 솔루션</h3>
        <p>Direct-to-Chip(D2C) 방식의 Cold Plate·CDU·열교환기 통합 시스템으로 초고집적 전자장비의 발열 문제를 해결합니다.</p>
        <a class="card-link" href="{{ '/technology/' | relative_url }}">기술 &amp; 제품 보기 →</a>
      </div>
      <div class="card">
        <div class="icon">🔬</div>
        <h3>실험장치 설계·제작</h3>
        <p>대학 및 기업 연구소를 위한 맞춤형 열유체 실험장치와 고정밀 계측 시스템을 설계하고 제작합니다.</p>
        <a class="card-link" href="{{ '/lab-solutions/' | relative_url }}">서비스 자세히 보기 →</a>
      </div>
      <div class="card">
        <div class="icon">🌐</div>
        <h3>Experimental World</h3>
        <p>실험 현장에서 쌓아온 실험기법과 계측장비에 대한 노하우를 소개하고 공유하는 지식 플랫폼입니다.</p>
        <a class="card-link" href="{{ '/experimental-world/' | relative_url }}">둘러보기 →</a>
      </div>
    </div>
  </div>
</section>

<section class="soft">
  <div class="container grid grid-2" style="align-items:center;">
    <div>
      <div class="eyebrow">Why Cooling Matters</div>
      <h2>발열 밀도가 높아질수록, 냉각은 선택이 아닌 필수입니다</h2>
      <p>GPU와 AI 가속기의 전력밀도는 매년 가파르게 증가하고 있습니다. 다수의 장비를 개별 공랭으로 식히는 방식은 한계에 부딪히고, 액체를 이용해 발열원 가까이에서 직접 열을 제거하는 방식이 필수가 되고 있습니다.</p>
      <p>프리거슨은 이 원리를 <strong>Direct-to-Chip(D2C)</strong> 방식으로 구현합니다. 칩 표면에 직접 맞닿는 Cold Plate와 냉각수를 순환·정화·제어하는 CDU, 그리고 최종 열교환기를 하나의 시스템으로 통합해 상용화 수준의 열관리 솔루션을 제공합니다.</p>
      <a class="btn btn-primary" href="{{ '/technology/' | relative_url }}">D2C 기술 자세히 보기</a>
    </div>
    <figure class="figure">
      <img src="{{ '/assets/images/concept-cooling.webp' | relative_url }}" alt="다수의 공랭식 PC 대비 액체 기반 냉각의 효율 비교 개념도">
      <figcaption>발열원을 개별 공랭 대신 액체 기반 시스템으로 통합하면 냉각 효율이 비약적으로 상승합니다. (개념도)</figcaption>
    </figure>
  </div>
</section>

<section>
  <div class="container">
    <blockquote class="quote-block">
      "1인기업에서 글로벌 딥테크 냉각기술 제조기업으로."<br>
      프리거슨은 청년 일자리를 창출하고 세계 최고 수준의 범용 냉각기술을 개발하여 글로벌 시장으로 도약합니다.
    </blockquote>
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
      <div class="eyebrow">Experimental World</div>
      <h2>최근 이야기</h2>
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
  <div class="container" style="text-align:center;">
    <h2>협업을 제안하거나 궁금한 점이 있으신가요?</h2>
    <p class="text-soft">냉각 솔루션 도입, 실험장치 제작 의뢰, 공동연구 제안 등 무엇이든 편하게 연락 주세요.</p>
    <a class="btn btn-primary" href="{{ '/contact/' | relative_url }}">문의하기</a>
  </div>
</section>
