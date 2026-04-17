---
layout: default
title: Case Studies
description: "Case studies by Soyoola Sodunke showing business problems, solution framing, and business-aligned technical thinking."
permalink: /case-studies/
---

# Case Studies

This page highlights practical work in a **case study format**. Each entry is intended to show more than a toolset. It should explain the customer context, the business problem, the solution path, and the commercial relevance of the recommendation.

## Selected Work

{% assign sorted_projects = site.projects | sort: "title" %}

{% if sorted_projects.size > 0 %}
<div class="card-grid">
  {% for project in sorted_projects %}
    {% include project-card.html project=project %}
  {% endfor %}
</div>
{% else %}
<p>No case studies have been published yet. Files added to the <code>_projects</code> collection will automatically appear here.</p>
{% endif %}

## What Each Case Study Should Prove

- the business problem was understood clearly
- the technical response matched the requirement
- the recommendation was framed in stakeholder language
- the outcome was anchored in business value

For presales work, that combination matters more than a raw feature list.
