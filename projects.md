---
layout: default
title: Projects
description: "Explore data analytics, business intelligence, and solution-focused projects by Soyoola Sodunke."
permalink: /projects/
---

# Projects

This section showcases selected projects that reflect my interest in **data analytics, business problem-solving, decision support, and solution-oriented thinking**.

The goal of these projects is not only to demonstrate technical ability, but also to show how data can be used to solve real business problems, support decision-making, and communicate insights clearly to stakeholders.

## What These Projects Represent

The projects featured here are designed to highlight strengths in areas such as:

- Business problem framing
- Data analysis and interpretation
- Dashboard and KPI thinking
- Reporting and decision support
- Structured problem-solving
- Solution communication
- Business-focused recommendations

## Project Portfolio

{% assign sorted_projects = site.projects | sort: "title" %}

{% if sorted_projects.size > 0 %}
<div class="card-grid">
  {% for project in sorted_projects %}
    {% include project-card.html project=project %}
  {% endfor %}
</div>
{% else %}
No projects have been published yet. Project entries added to the `_projects` folder will automatically appear here.
{% endif %}

## Related Content

You may also be interested in the technical articles section, where I share writeups on analytics, business intelligence, solution engineering, and related technical concepts.

[Read Articles]({{ '/articles/' | relative_url }})
