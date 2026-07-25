---
layout: page
lang: en
title: Archive
subtitle: Experimental World — a record of experimental techniques and measurement instrumentation.
permalink: /en/experimental-world/
alt_url: /experimental-world/
description: "FRIGUSON's Archive (Experimental World) records and shares know-how on thermal-fluid experimental techniques and measurement instrumentation."
---

<section style="padding-top:0;">
  <p style="max-width:720px;">Archive (Experimental World) is where FRIGUSON records and shares the experimental techniques and instrumentation know-how we've built up in the field and in research. We share what we've learned from designing and instrumenting thermal-fluid experiments with universities, research institutes, and fellow engineers.</p>

  {% assign posts = site.experiments_en | sort: "date" | reverse %}
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
        <div class="meta">{{ post.date | date: "%b %d, %Y" }}</div>
      </div>
    </a>
    {% endfor %}
  </div>
  {% else %}
  <p class="text-soft">Our first article is coming soon.</p>
  {% endif %}
</section>
