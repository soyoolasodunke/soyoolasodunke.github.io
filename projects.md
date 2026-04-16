---
layout: default
title: Projects
description: "Explore data analytics, business intelligence, and solution-focused projects by Soyoola Sodunke."
permalink: /projects/
---

# Projects

This section showcases selected projects that reflect my interest in **business problem-solving and solution-oriented thinking**. The goal here is not only to demonstrate technical ability, but also to show how data can be used to solve real business problems, support decision-making, and communicate insights clearly to stakeholders.

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

You may also be interested in the articles section, where I give practical perspectives on solving enterprise data challenges, with a focus on data foundations, governance, trust, and informed technology decisions.

[Read Articles]({{ '/articles/' | relative_url }})
