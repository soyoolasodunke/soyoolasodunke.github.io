---
layout: default
title: Home
description: "Portfolio of data analytics projects, technical writeups, and solution-focused work by Soyoola Sodunke, Presales Engineer and Data Solutions Engineer."
---

## What I Do

I help organizations solve business problems with **data analytics, and solution-oriented thinking**. My work focuses on translating business needs into clear technical direction through problem discovery, technical proposals, value proposition demos, and practical solution communication.

<div class="card-grid">
  <div class="card">
    <h3>Data Analytics Projects</h3>
    <p>I build and document projects that demonstrate business problem-solving, KPI thinking, reporting logic, dashboard design, and decision support.</p>
    <p><a href="{{ '/projects/' | relative_url }}">Explore Projects →</a></p>
  </div>

  <div class="card">
    <h3>Technical Articles</h3>
    <p>I write clear and practical articles on data modernization, AI/ML transformation, data platforms implementation, and presales engineering concepts.</p>
    <p><a href="{{ '/articles/' | relative_url }}">Read Articles →</a></p>
  </div>

  <div class="card">
    <h3>Solution Engineering Mindset</h3>
    <p>I approach technical work with a strong focus on clarity, business value, customer relevance, and practical implementation.</p>
  </div>
</div>


## Featured Projects

{% assign featured_projects = site.projects | where: "featured", true %}

{% if featured_projects.size > 0 %}
<div class="card-grid">
  {% for project in featured_projects limit:3 %}
    {% include project-card.html project=project %}
  {% endfor %}
</div>
{% else %}
<p>No featured projects yet. Mark any project with <code>featured: true</code> in its front matter to show it here.</p>
{% endif %}

<p><a href="{{ '/projects/' | relative_url }}">View All Projects →</a></p>

## Latest Articles

{% if site.posts.size > 0 %}
<div class="card-grid">
  {% for post in site.posts limit:3 %}
    {% include article-card.html post=post %}
  {% endfor %}
</div>
{% else %}
<p>No articles published yet. Posts added to the <code>_posts</code> folder will appear here automatically.</p>
{% endif %}

<p><a href="{{ '/articles/' | relative_url }}">View All Articles →</a></p>

## Why This Portfolio

This site is designed to showcase how I think through business and technical problems, communicate clearly, and structure practical data-driven solutions. It reflects both my technical interests and my professional direction as a customer-facing engineer.
