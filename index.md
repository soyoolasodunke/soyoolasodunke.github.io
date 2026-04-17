---
layout: default
title: Home
description: "Presales portfolio of Soyoola Sodunke, focused on case studies, solution methodology, and business-aligned Data & AI advisory."
---

<div class="card-grid home-overview-grid">
  <div class="card">
    <h3>Case Studies</h3>
    <p>Selected work showing business context, solution framing, technical credibility, and decision-ready outcomes.</p>
    <p><a href="{{ '/case-studies/' | relative_url }}">Explore Case Studies →</a></p>
  </div>

  <div class="card">
    <h3>Methodology</h3>
    <p>A practical presales approach for discovery, qualification, solution mapping, and value articulation.</p>
    <p><a href="{{ '/methodology/' | relative_url }}">View Methodology →</a></p>
  </div>

  <div class="card">
    <h3>Insights</h3>
    <p>Short essays on Data, AI, architecture, and how technical choices connect to business decisions.</p>
    <p><a href="{{ '/insights/' | relative_url }}">Read Insights →</a></p>
  </div>
</div>

## Sales Impact

<div class="card-grid two-up impact-grid home-impact-grid">
  <div class="card impact-card">
    <p class="card-kicker">Discovery</p>
    <h3>Clearer Problem Definition</h3>
    <p>I help commercial teams move beyond surface requirements and get to the real business issue, constraints, and buying context.</p>
  </div>
  <div class="card impact-card">
    <p class="card-kicker">Solution Framing</p>
    <h3>Credible Technical Direction</h3>
    <p>I shape architectures, demos, and narratives that reduce uncertainty and make the recommendation easier to trust.</p>
  </div>
  <div class="card impact-card">
    <p class="card-kicker">Stakeholder Alignment</p>
    <h3>Executive and Technical Relevance</h3>
    <p>I adapt the same solution story for business sponsors and technical evaluators without losing precision.</p>
  </div>
  <div class="card impact-card">
    <p class="card-kicker">Business Value</p>
    <h3>Decision-Ready Value Narrative</h3>
    <p>I connect capabilities to outcomes such as speed, efficiency, visibility, risk reduction, and revenue potential.</p>
  </div>
</div>

## Recent Insights

{% if site.posts.size > 0 %}
<div class="card-grid">
  {% for post in site.posts limit:3 %}
    {% include article-card.html post=post %}
  {% endfor %}
</div>
{% else %}
<p>No insights published yet. Content added to the <code>_posts</code> folder will appear here automatically.</p>
{% endif %}

<p><a href="{{ '/insights/' | relative_url }}">Browse All Insights →</a></p>
