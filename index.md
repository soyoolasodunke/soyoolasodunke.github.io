---
layout: default
title: Home
description: "Presales portfolio of Soyoola Sodunke, focused on case studies, solution methodology, and business-aligned Data & AI advisory."
---

## Why This Site Exists

I built this portfolio to demonstrate a **presales engineering operating model**, not just technical interest. The emphasis is on how I approach customer problems, shape solution direction, and communicate the commercial value of Data &amp; AI initiatives with clarity.

<div class="card-grid">
  <div class="card">
    <h3>Case Studies</h3>
    <p>Structured examples that show the business problem, the solution path, the technical considerations, and the outcome the customer cared about.</p>
    <p><a href="{{ '/case-studies/' | relative_url }}">Explore Case Studies →</a></p>
  </div>

  <div class="card">
    <h3>Methodology</h3>
    <p>A repeatable approach for discovery, qualification, solution mapping, technical storytelling, and value articulation across enterprise engagements.</p>
    <p><a href="{{ '/methodology/' | relative_url }}">View Methodology →</a></p>
  </div>

  <div class="card">
    <h3>Insights</h3>
    <p>Thought pieces that translate technical topics into practical, decision-oriented narratives for business and technical stakeholders.</p>
    <p><a href="{{ '/insights/' | relative_url }}">Read Insights →</a></p>
  </div>
</div>

## What I Bring to an Engagement

<div class="card-grid two-up">
  <div class="card">
    <h3>Commercially Aligned Technical Thinking</h3>
    <p>I focus on aligning architecture, implementation paths, and technical trade-offs to the commercial objectives of the opportunity.</p>
  </div>
  <div class="card">
    <h3>Audience-Centric Communication</h3>
    <p>I adapt the same solution for executive buyers, business sponsors, and technical evaluators without losing precision or relevance.</p>
  </div>
  <div class="card">
    <h3>Structured Discovery</h3>
    <p>I prioritize problem framing, current-state understanding, constraints, and decision criteria before pushing products or tooling.</p>
  </div>
  <div class="card">
    <h3>Business Value Translation</h3>
    <p>I work to connect technical capability to measurable outcomes such as risk reduction, speed, visibility, efficiency, or revenue potential.</p>
  </div>
</div>

## Featured Case Study

{% assign featured_projects = site.projects | where: "featured", true %}

{% if featured_projects.size > 0 %}
<div class="card-grid">
  {% for project in featured_projects limit:3 %}
    {% include project-card.html project=project %}
  {% endfor %}
</div>
{% else %}
<p>Add <code>featured: true</code> to a case study in the <code>_projects</code> collection to surface it here.</p>
{% endif %}

<p><a href="{{ '/case-studies/' | relative_url }}">View All Case Studies →</a></p>

## My Presales Flow

<div class="process-grid">
  <div class="process-step">
    <span class="process-number">01</span>
    <h3>Discover</h3>
    <p>Clarify the business driver, the current pain, the stakeholders, and the decision environment.</p>
  </div>
  <div class="process-step">
    <span class="process-number">02</span>
    <h3>Frame</h3>
    <p>Translate requirements into a clear solution hypothesis with the right scope, assumptions, and success criteria.</p>
  </div>
  <div class="process-step">
    <span class="process-number">03</span>
    <h3>Prove</h3>
    <p>Use architecture, demos, narratives, and technical validation to reduce buyer uncertainty.</p>
  </div>
  <div class="process-step">
    <span class="process-number">04</span>
    <h3>Quantify</h3>
    <p>Connect the recommendation to business value, adoption logic, and implementation credibility.</p>
  </div>
</div>

<p><a href="{{ '/methodology/' | relative_url }}">Read the Full Methodology →</a></p>

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

## Next Conversation

If you are evaluating a presales engineer, solution consultant, or Data &amp; AI advisory profile, this site should give you three things quickly: how I think, how I communicate, and how I shape technical work into decision-ready business narratives.
