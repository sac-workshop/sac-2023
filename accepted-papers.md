---
layout: default
title: Accepted papers
---

# Accepted papers

{% if site.data.variables.show_accepted_papers %}

<ul>

{% for paper in site.data.accepted_papers %}

<li class="mt-3 mb-3">
<b>{{ paper.title }}</b> – {{ paper.authors }}
{% if site.data.variables.show_preproceedings_links and paper.preproceeding %}
• <a href="{{ paper.preproceeding }}">pre-proceeding version (PDF)</a>
{% endif %}
</li>

{% endfor %}

</ul>

{% endif %}