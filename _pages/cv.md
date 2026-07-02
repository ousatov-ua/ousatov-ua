---
title: "CV"
permalink: /cv/
description: "Experience, projects, skills, certifications, education, and patents."
---
{% assign profile = site.data.profile %}

{{ profile.title }} - {{ profile.location }}

## Skills

{% for skill in profile.skills %}
- {{ skill }}
{% endfor %}

## Selected Impact

{% for highlight in profile.highlights %}
- {{ highlight }}
{% endfor %}

## Experience

{% for job in site.data.experience %}
### {{ job.role }}
{{ job.organization }} - {{ job.location }} - {{ job.start }}-{{ job.end }}

{% for highlight in job.highlights %}
- {{ highlight }}
{% endfor %}

{% endfor %}

## Projects

{% for project in site.data.projects %}
- **{{ project.title }}** - {{ project.summary }}
{% endfor %}

## Certifications

{% for certification in profile.certifications %}
- **{{ certification.title }}**, {{ certification.issuer }} ({{ certification.issued }})
{% endfor %}

## Education

{% for education in profile.education %}
- {{ education }}
{% endfor %}

## Languages

{% for language in profile.languages %}
- {{ language }}
{% endfor %}

## Patents

{% for patent in profile.patents %}
- **{{ patent.title }}**{% if patent.number %}, {{ patent.number }}{% endif %}{% if patent.issued %}, issued {{ patent.issued }}{% endif %}
{% endfor %}
