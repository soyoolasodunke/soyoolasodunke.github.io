---
layout: default
title: Articles
description: "Read technical articles and writeups by Soyoola Sodunke on analytics, business intelligence, data platforms, and presales engineering."
permalink: /articles/
---

# Articles

This section contains technical writeups and professional articles focused on **analytics, business intelligence, data solutions, and presales engineering**.

The purpose of these articles is to explain ideas clearly, simplify technical concepts, and share practical thinking that can help professionals, stakeholders, and decision-makers better understand modern data and solution topics.

## What You Will Find Here

The articles on this site are written to be:

- Clear and easy to understand
- Practical and professionally relevant
- Focused on real business and technical questions
- Useful for both technical and non-technical readers
- Grounded in solution-oriented thinking

## Main Topics Covered

### Data Analytics
Articles in this category explore how data can be used to generate insight, support decision-making, and improve business visibility.

### Business Intelligence
These articles focus on common BI concepts, tool logic, and practical understanding.

### Data Platforms and Solution Design
These writeups explore broader solution and architecture ideas relevant to modern organizations.

### Presales Engineering
This category focuses on the customer-facing technical profession itself.

## Why These Articles Matter

Strong technical work becomes far more valuable when it can be explained clearly. In customer-facing roles like presales and solution engineering, the ability to communicate technical ideas simply is just as important as understanding the technology itself.

These articles reflect that belief. They are intended to show not only what I know, but also how I think and how I communicate.

## Published Articles

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
  ### [{{ post.title }}]({{ post.url | relative_url }})

  **Published:** {{ post.date | date: "%B %d, %Y" }}

  {% if post.description %}
  {{ post.description }}
  {% elsif post.excerpt %}
  {{ post.excerpt | strip_html | truncate: 220 }}
  {% else %}
  A technical article on analytics, business intelligence, solution design, or presales engineering.
  {% endif %}

  ---
  {% endfor %}
{% else %}
No articles have been published yet. New posts added to the `_posts` folder will automatically appear here.
{% endif %}

## Explore My Project Work

If you would like to see practical examples of how these ideas are applied, please visit the projects section.

[View Projects]({{ '/projects/' | relative_url }})
