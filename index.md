---
layout: home
title: ML System Design
nav_exclude: true
seo:
  type: Курс
  name: Дослідження і проектування інтелектуальних систем
---

# {{ site.tagline }}
{: .mb-2 }
{{ site.description }}
{: .fs-6 .fw-300 }

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign overview = site.slides | where: "title", "Огляд" | first %}
{{ overview.content }}

<small>[Більше..]({{ site.baseurl }}{% link about.md %})</small>

{% for module in site.modules %}
{{ module }}
{% endfor %}
