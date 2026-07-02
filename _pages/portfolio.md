---
title: "Projects"
permalink: /portfolio/
description: "Selected backend, distributed systems, AI-agent infrastructure, and developer tooling projects."
---

{% for project in site.data.projects %}
## {{ project.title }}

{{ project.summary }}

{% if project.tags %}
Tags: {{ project.tags | join: ", " }}
{% endif %}

{% if project.url %}[Project]({{ project.url }}){% endif %}
{% if project.repo %}[Repository]({{ project.repo }}){% endif %}
{% endfor %}
