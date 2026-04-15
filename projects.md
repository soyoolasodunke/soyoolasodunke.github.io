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

Each project is approached with a practical mindset: understand the problem, work through the data, generate insight, and present findings in a way that is meaningful to decision-makers.

## Project Categories

### Data Analytics Projects
Projects in this category focus on using data to answer business questions, identify patterns, and support better decisions.

### Business Intelligence and Reporting
These projects focus on how data should be structured, presented, and used in reporting environments.

### Solution and Case-Based Projects
These projects demonstrate solution thinking, especially where business needs must be translated into a technical or analytical response.

## Why This Matters

As a Presales Engineer and Data Solutions Engineer, I believe projects should do more than display tools or charts. They should demonstrate structured thinking, clarity of communication, and the ability to connect analysis to business value.

That is the standard these projects aim to meet.

## Project Portfolio

{% assign sorted_projects = site.projects | sort: "title" %}

{% if sorted_projects.size > 0 %}
  {% for project in sorted_projects %}
  ### [{{ project.title }}]({{ project.url | relative_url }})

  {% if project.summary %}
  {{ project.summary }}
  {% elsif project.description %}
  {{ project.description }}
  {% else %}
  A project focused on business problem-solving, analytics, and solution-oriented thinking.
  {% endif %}

  {% if project.tools %}
  **Tools:** {{ project.tools | join: ", " }}
  {% endif %}

  {% if project.business_problem %}
  **Business Problem:** {{ project.business_problem }}
  {% endif %}

  ---
  {% endfor %}
{% else %}
No projects have been published yet. Project entries added to the `_projects` folder will automatically appear here.
{% endif %}

## Related Content

You may also be interested in the technical articles section, where I share writeups on analytics, business intelligence, solution engineering, and related technical concepts.

[Read Articles]({{ '/articles/' | relative_url }})
