---
layout: default
title: Insights
description: "Technical and commercial insights by Soyoola Sodunke on Data, AI, solution engineering, and business-focused technology advisory."
permalink: /insights/
---

# Insights

These articles are written to make technical topics more decision-useful. The intent is not just to explain technology, but to connect it to customer priorities, transformation choices, and solution design implications.

## Published Insights

{% if site.posts.size > 0 %}
<div class="card-grid">
  {% for post in site.posts %}
    {% include article-card.html post=post %}
  {% endfor %}
</div>
{% else %}
<p>No insights have been published yet. New posts added to the <code>_posts</code> folder will appear here automatically.</p>
{% endif %}

## Also Explore

For applied examples, visit the [Case Studies]({{ '/case-studies/' | relative_url }}) section.
