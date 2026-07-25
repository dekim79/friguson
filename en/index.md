---
layout: home
lang: en
title: "FRIGUSON — A Workshop for High-Heat-Flux Cooling"
description: "Friguson Co., Ltd. is a cooling workshop that designs and builds Direct-to-Chip (D2C) systems based on phase-change heat transfer, and fabricates experimental apparatus for university and corporate research labs."
permalink: /en/
alt_url: /
hero_tagline: "General Purpose Technology for Cooling"
hero_title: "We remove high heat flux right where it happens."
hero_lead: "FRIGUSON is a cooling workshop redesigning the thermal limits of ultra-high-density GPUs and power semiconductors with Direct-to-Chip (D2C) systems built on phase-change heat transfer."
hero_primary_label: "See the Workbench"
hero_primary_url: /en/workbench/
hero_secondary_label: "Commission a build"
hero_secondary_url: /en/workshop/
hero_image: /assets/images/diagram-d2c-system.png
hero_image_alt: "D2C cooling system concept — Cold Plate, CDU, final heat exchanger"
hero_image_caption: "The Cold Plate absorbs heat directly at the chip surface. (To be replaced with real photos and IR thermal imaging.)"
---

<section>
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">The Workshop</div>
      <h2>Step into the workshop</h2>
      <p class="text-soft">A space for building what isn't sold off the shelf — and can't be.</p>
    </div>
    <div class="grid grid-4">
      <div class="card">
        <h3>Workbench</h3>
        <p>A log of what we're building, and what we've already built.</p>
        <a class="card-link" href="{{ '/en/workbench/' | relative_url }}">See the log →</a>
      </div>
      <div class="card">
        <h3>Toolshop</h3>
        <p>Finished parts and equipment, sold at a set price.</p>
        <a class="card-link" href="{{ '/en/toolshop/' | relative_url }}">Browse the shop →</a>
      </div>
      <div class="card">
        <h3>Workshop</h3>
        <p>We design and build experimental apparatus that doesn't exist yet.</p>
        <a class="card-link" href="{{ '/en/workshop/' | relative_url }}">Commission a build →</a>
      </div>
      <div class="card">
        <h3>Archive</h3>
        <p>A record of experimental techniques and instrumentation know-how.</p>
        <a class="card-link" href="{{ '/en/experimental-world/' | relative_url }}">Read the archive →</a>
      </div>
    </div>
  </div>
</section>

<section class="soft">
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">From the Workbench</div>
      <h2>What we're building right now</h2>
    </div>
    <div class="grid grid-2" style="align-items:center;">
      <figure class="figure">
        <img src="{{ '/assets/images/diagram-rd-roadmap.png' | relative_url }}" alt="5-stage R&D roadmap">
        <figcaption>Stage 1 Theoretical analysis → Stage 5 Comprehensive evaluation &amp; commercialization verification</figcaption>
      </figure>
      <div>
        <span class="status-pill status-ongoing">Ongoing</span>
        <h3 style="margin-top:14px;">D2C High-Heat-Flux Cooling System</h3>
        <p>Cold Plate, CDU, final heat exchanger, sensors &amp; control — four technology elements, pushed toward commercialization.</p>
        <a class="btn btn-outline" href="{{ '/en/workbench/' | relative_url }}">See the full build log</a>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">Track Record</div>
      <h2>What's on record</h2>
    </div>
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
      <div class="eyebrow">Archive</div>
      <h2>Latest from the Archive</h2>
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
  <div class="container">
    <div class="section-head">
      <div class="eyebrow">Toolshop</div>
      <h2>A look at the shop</h2>
    </div>
    <div class="grid grid-3">
      <div class="card shop-card">
        <div class="shop-thumb">Photo coming soon</div>
        <h3>D2C Cold Plate Module</h3>
        <div class="shop-price">Contact for pricing</div>
      </div>
      <div class="card shop-card">
        <div class="shop-thumb">Photo coming soon</div>
        <h3>Compact CDU</h3>
        <div class="shop-price">Contact for pricing</div>
      </div>
      <div class="card shop-card">
        <div class="shop-thumb">Photo coming soon</div>
        <h3>D2C Integrated Package</h3>
        <div class="shop-price">Contact for pricing</div>
      </div>
    </div>
    <div style="text-align:center; margin-top:32px;">
      <a class="btn btn-outline" href="{{ '/en/toolshop/' | relative_url }}">Browse the full Toolshop</a>
    </div>
  </div>
</section>

<section class="soft">
  <div class="container" style="text-align:center;">
    <h2>Want to build something that doesn't exist yet?</h2>
    <p class="text-soft">Design, fabrication, theory, and academic discussion — we build it with you from the idea stage.</p>
    <a class="btn btn-primary" href="{{ '/en/workshop/' | relative_url }}">Commission a build</a>
  </div>
</section>
