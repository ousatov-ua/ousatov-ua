---
title: "About"
permalink: /about/
description: "Lead Backend Engineer focused on reliable distributed platforms, event-driven systems, and AI-agent infrastructure."
---
{% assign profile = site.data.profile %}

{{ profile.tagline }}

{% for item in profile.summary %}
{{ item }}

{% endfor %}

## Core Skills

{% for skill in profile.skills %}
- {{ skill }}
{% endfor %}

## Selected Impact

{% for highlight in profile.highlights %}
- {{ highlight }}
{% endfor %}

## Focus Areas

{% for interest in profile.interests %}
- {{ interest }}
{% endfor %}

## Working Style

{% for item in profile.social_proof %}
- {{ item }}
{% endfor %}
