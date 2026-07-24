---
layout: home
lang: en
title: "FRIGUSON | Electronics Cooling Solutions"
description: "FRIGUSON Inc. develops high-efficiency, low-carbon Direct-to-Chip (D2C) cooling solutions for high-density electronics, and designs experimental apparatus for university and corporate research labs."
permalink: /en/
alt_url: /
hero_tagline: "General Purpose Technology for Cooling"
hero_title: "Setting a new standard for electronics cooling with Direct-to-Chip thermal management"
hero_lead: "FRIGUSON is a thermal-fluid engineering deep-tech company that designs and manufactures high-efficiency, low-carbon cooling systems for ultra-high-density GPUs, power semiconductors, and AI servers."
hero_primary_label: "Explore Technology"
hero_primary_url: /en/technology/
hero_secondary_label: "Request Lab Equipment"
hero_secondary_url: /en/lab-solutions/
---

<section>
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">Business</div>
      <h2>What FRIGUSON Does</h2>
      <p class="text-soft">We build value across three business areas, grounded in our core cooling technology.</p>
    </div>
    <div class="grid grid-3">
      <div class="card">
        <div class="icon">❄</div>
        <h3>Electronics Cooling Solutions</h3>
        <p>Integrated Cold Plate, CDU, and heat exchanger systems built on Direct-to-Chip (D2C) technology to solve the thermal challenges of ultra-high-density electronics.</p>
        <a class="card-link" href="{{ '/en/technology/' | relative_url }}">See Technology →</a>
      </div>
      <div class="card">
        <div class="icon">🔬</div>
        <h3>Lab Equipment Design &amp; Fabrication</h3>
        <p>We design and build custom thermal-fluid experimental apparatus and high-precision measurement systems for university and corporate research labs.</p>
        <a class="card-link" href="{{ '/en/lab-solutions/' | relative_url }}">See Services →</a>
      </div>
      <div class="card">
        <div class="icon">🌐</div>
        <h3>Experimental World</h3>
        <p>A knowledge platform where we share hands-on know-how on experimental techniques and measurement instrumentation.</p>
        <a class="card-link" href="{{ '/en/experimental-world/' | relative_url }}">Explore →</a>
      </div>
    </div>
  </div>
</section>

<section class="soft">
  <div class="container grid grid-2" style="align-items:center;">
    <div>
      <div class="eyebrow">Why Cooling Matters</div>
      <h2>As power density rises, cooling becomes essential, not optional</h2>
      <p>The power density of GPUs and AI accelerators is climbing sharply every year. Cooling many devices individually with air reaches its limit, making liquid-based cooling that removes heat right at the source essential.</p>
      <p>FRIGUSON implements this principle through <strong>Direct-to-Chip (D2C)</strong> cooling. We integrate a Cold Plate that contacts the chip directly, a CDU that circulates, purifies, and controls coolant, and a final heat exchanger into a single commercialization-ready thermal management system.</p>
      <a class="btn btn-primary" href="{{ '/en/technology/' | relative_url }}">Learn about D2C technology</a>
    </div>
    <figure class="figure">
      <img src="{{ '/assets/images/concept-cooling.webp' | relative_url }}" alt="Concept comparison of many air-cooled desktop PCs versus a single liquid-cooled system">
      <figcaption>Consolidating many air-cooled heat sources into a single liquid-based system dramatically improves cooling efficiency. (Concept illustration)</figcaption>
    </figure>
  </div>
</section>

<section>
  <div class="container">
    <blockquote class="quote-block">
      "From a one-person startup to a global deep-tech cooling technology manufacturer."<br>
      FRIGUSON aims to create jobs for young engineers and develop world-class general-purpose cooling technology to reach the global market.
    </blockquote>
    <div class="stat-row">
      <div class="stat"><span class="num">20+</span><span class="label">years of thermal-fluid research (CEO)</span></div>
      <div class="stat"><span class="num">40+</span><span class="label">SCI-indexed publications</span></div>
      <div class="stat"><span class="num">Top 2%</span><span class="label">World Top 2% Scientist</span></div>
      <div class="stat"><span class="num">PUE 1.1</span><span class="label">target system energy-efficiency</span></div>
    </div>
  </div>
</section>

{% assign latest = site.experiments_en | sort: "date" | reverse %}
{% if latest.size > 0 %}
<section class="soft">
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">Experimental World</div>
      <h2>Latest Stories</h2>
      <p class="text-soft">Read our latest articles on experimental techniques and measurement instrumentation.</p>
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
          <div class="meta">{{ post.date | date: "%b %d, %Y" }}</div>
        </div>
      </a>
      {% endfor %}
    </div>
  </div>
</section>
{% endif %}

<section>
  <div class="container" style="text-align:center;">
    <h2>Have a project or question in mind?</h2>
    <p class="text-soft">Whether it's adopting a cooling solution, commissioning lab equipment, or proposing a collaboration — feel free to reach out.</p>
    <a class="btn btn-primary" href="{{ '/en/contact/' | relative_url }}">Get in touch</a>
  </div>
</section>
