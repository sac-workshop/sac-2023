---
layout: default
title: Accepted papers
---

# Accepted papers

{% if site.data.variables.show_accepted_papers %}

<ul>

{% for paper in site.data.accepted_papers %}

<li class="mt-3 mb-3"><b>{{ paper.title }}</b> – {{ paper.authors }}</li>

{% endfor %}

</ul>

{% endif %}