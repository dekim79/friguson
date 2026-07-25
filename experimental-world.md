---
layout: page
lang: ko
title: Archive
subtitle: 서재 — Experimental World. 실험기법과 계측장비에 대한 지식을 기록하고 공유합니다.
permalink: /experimental-world/
alt_url: /en/experimental-world/
description: "열유체 실험기법과 계측장비에 대한 프리거슨의 노하우를 기록하고 공유하는 서재, Experimental World 입니다."
---

<section style="padding-top:0;">
  <p style="max-width:720px;">Archive(Experimental World)는 프리거슨이 실무와 연구 현장에서 쌓아온 실험기법과 계측장비 노하우를 기록하고 공유하는 서재입니다. 열유체 실험을 설계하고 계측하는 과정에서 얻은 지식을 대학, 연구소, 엔지니어 여러분과 나눕니다.</p>

  {% assign posts = site.experiments_ko | sort: "date" | reverse %}
  {% if posts.size > 0 %}
  <div class="article-grid" style="margin-top:40px;">
    {% for post in posts %}
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
  {% else %}
  <p class="text-soft">곧 첫 번째 글이 올라올 예정입니다.</p>
  {% endif %}
</section>
