---
layout: default
title: Articles
description: "Read technical articles and writeups by Soyoola Sodunke on analytics, business intelligence, data platforms, and presales engineering."
permalink: /articles/
---

# Articles

This section features technical articles and professional insights focused on data, analytics, AI-driven solutions, and presales engineering practices.

The content is designed to translate complex technologies into clear, business-relevant narratives that support informed decision-making. It emphasizes practical solution thinking, real-world application, and the alignment of data and AI capabilities with business outcomes.

Reflecting the core responsibility of a presales engineer, these writeups demonstrate not only technical depth, but the ability to structure, simplify, and communicate solutions effectively to both technical and non-technical stakeholders.

## Published Articles

{% if site.posts.size > 0 %}
<div class="card-grid">
  {% for post in site.posts %}
    {% include article-card.html post=post %}
  {% endfor %}
</div>
{% else %}
No articles have been published yet. New posts added to the `_posts` folder will automatically appear here.
{% endif %}

## Explore My Project Work

Would you like to see practical examples of how these ideas are applied? Please visit my projects section.

[View Projects]({{ '/projects/' | relative_url }})
