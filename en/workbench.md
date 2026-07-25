---
layout: page
lang: en
title: Workbench
subtitle: A log of what we're building, and what we've already built.
permalink: /en/workbench/
alt_url: /workbench/
description: "A build log of the high-heat-flux cooling system and custom projects FRIGUSON is designing and fabricating — the Workbench."
---

<section style="padding-top:0;">
  <div class="eyebrow">Workbench</div>
  <h2>Built, and being built</h2>
  <p>Workbench is a record of what FRIGUSON has been commissioned to build, and what we're building on our own. Left as results, not explanations.</p>
</section>

<section class="soft log-entry">
  <div class="log-head">
    <span class="status-pill status-ongoing">Ongoing</span>
    <div class="eyebrow" style="margin:0;">Flagship Project</div>
  </div>
  <h2>D2C High-Heat-Flux Cooling System</h2>
  <p>A Direct-to-Chip (D2C) system that removes heat as close as possible to the source. By using phase-change heat transfer, it handles far higher heat flux, more reliably, than cooling many devices individually with air. Built around four core technology elements.</p>

  <div class="grid grid-2" style="margin-top:24px;">
    <div class="card">
      <h3>1. Cold Plate Design &amp; Manufacturing</h3>
      <p>We optimize microchannel-based flow structures and materials to fabricate the core heat-dissipation component mounted directly on high-heat chipsets.</p>
    </div>
    <div class="card">
      <h3>2. CDU (Coolant Distribution Unit)</h3>
      <p>We design and build coolant distribution units that compactly integrate pumps, heat exchangers, water-purification filters, and control logic.</p>
    </div>
    <div class="card">
      <h3>3. Final Heat Exchanger &amp; System Design</h3>
      <p>We select air- or liquid-cooled final heat exchangers and design the entire cooling loop as a single integrated system.</p>
    </div>
    <div class="card">
      <h3>4. Sensors &amp; Control Systems</h3>
      <p>Thermocouple- and DAQ-based precision temperature measurement, together with flow and pressure control, ensure operational stability and uniform cooling performance.</p>
    </div>
  </div>

  <figure class="figure" style="margin-top:32px;">
    <img src="{{ '/assets/images/diagram-d2c-system.png' | relative_url }}" alt="D2C integrated system concept: high-performance Cold Plate, CDU, and final heat exchanger connections">
    <figcaption>D2C integrated system concept — Cold Plate ↔ CDU ↔ final heat exchanger (to be replaced with real photos and IR thermal imaging)</figcaption>
  </figure>

  <figure class="figure" style="margin-top:20px;">
    <img src="{{ '/assets/images/diagram-rd-roadmap.png' | relative_url }}" alt="5-stage R&D roadmap: theoretical analysis, Cold Plate design, prototyping, performance testing, comprehensive evaluation">
    <figcaption>Stage 1 Theoretical analysis → Stage 2 Cold Plate optimal design → Stage 3 Prototyping → Stage 4 Performance testing &amp; verification → Stage 5 Comprehensive evaluation &amp; commercialization verification</figcaption>
  </figure>

  <ul class="badge-list" style="margin-top:24px;">
    <li class="badge">AI &amp; Data Centers</li>
    <li class="badge">Power Semiconductors</li>
    <li class="badge">Future Mobility Electronics</li>
    <li class="badge">PUE 1.1 target</li>
  </ul>

  <a class="btn btn-primary" href="{{ '/en/toolshop/' | relative_url }}" style="margin-top:8px;">Finished parts are in the Toolshop →</a>
</section>

<section>
  <div class="eyebrow">Next</div>
  <h2>What's Next</h2>
  <div class="grid grid-2">
    <div class="card log-placeholder">
      <span class="status-pill status-soon">Coming soon</span>
      <h3>Next build log</h3>
      <p class="text-soft">New build entries are added continuously.</p>
    </div>
    <div class="card log-placeholder">
      <span class="status-pill status-soon">Coming soon</span>
      <h3>Next build log</h3>
      <p class="text-soft">New build entries are added continuously.</p>
    </div>
  </div>
</section>

<section class="soft" style="text-align:center;">
  <h2>Your project could be on this bench too</h2>
  <p class="text-soft">If you want to build something that isn't sold off the shelf — and can't be — we design it together in Workshop.</p>
  <a class="btn btn-primary" href="{{ '/en/workshop/' | relative_url }}">Commission a build</a>
</section>
