---
layout: default
title: Accepted papers
---

<script>
window.addEventListener('load', function() {
  const tooltipTriggerList = document.querySelectorAll('[data-bs-toggle="tooltip"]')
  const tooltipList = [...tooltipTriggerList].map(tooltipTriggerEl => new bootstrap.Tooltip(tooltipTriggerEl))
})
</script>

# Accepted papers

{% if site.data.variables.show_accepted_papers %}

<ul>

{% for paper in site.data.accepted_papers %}

<li class="mt-3 mb-3">
<b>{{ paper.title }}</b> – <span class="me-2">{{ paper.authors }}</span>
{% if site.data.variables.show_preproceedings_links and paper.preproceeding %}
<br />
{% elsif site.data.variables.show_proceedings_link and paper.doi %}
<br />
{% elsif site.data.variables.show_slides_links and paper.slides %}
<br />
{% endif %}
{% if site.data.variables.show_preproceedings_links and paper.preproceeding %}
<a class="btn btn-outline-primary btn-sm d-print-none talk-btn" href="{{ paper.preproceeding }}" data-bs-toggle="tooltip" data-bs-placement="bottom" data-bs-title="Pre-proceeding version">
<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-file-earmark-text" viewBox="0 0 16 16">
    <path d="M5.5 7a.5.5 0 0 0 0 1h5a.5.5 0 0 0 0-1zM5 9.5a.5.5 0 0 1 .5-.5h5a.5.5 0 0 1 0 1h-5a.5.5 0 0 1-.5-.5m0 2a.5.5 0 0 1 .5-.5h2a.5.5 0 0 1 0 1h-2a.5.5 0 0 1-.5-.5"/>
    <path d="M9.5 0H4a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h8a2 2 0 0 0 2-2V4.5zm0 1v2A1.5 1.5 0 0 0 11 4.5h2V14a1 1 0 0 1-1 1H4a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1z"/>
</svg>
</a>
{% endif %}
{% if site.data.variables.show_proceedings_link and paper.doi %}
<a class="btn btn-outline-primary btn-sm d-print-none talk-btn" href="https://doi.org/{{ paper.doi }}" data-bs-toggle="tooltip" data-bs-placement="bottom" data-bs-title="Published version">
<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-journal-text" viewBox="0 0 16 16">
<path d="M5 10.5a.5.5 0 0 1 .5-.5h2a.5.5 0 0 1 0 1h-2a.5.5 0 0 1-.5-.5m0-2a.5.5 0 0 1 .5-.5h5a.5.5 0 0 1 0 1h-5a.5.5 0 0 1-.5-.5m0-2a.5.5 0 0 1 .5-.5h5a.5.5 0 0 1 0 1h-5a.5.5 0 0 1-.5-.5m0-2a.5.5 0 0 1 .5-.5h5a.5.5 0 0 1 0 1h-5a.5.5 0 0 1-.5-.5"/>
<path d="M3 0h10a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2v-1h1v1a1 1 0 0 0 1 1h10a1 1 0 0 0 1-1V2a1 1 0 0 0-1-1H3a1 1 0 0 0-1 1v1H1V2a2 2 0 0 1 2-2"/>
<path d="M1 5v-.5a.5.5 0 0 1 1 0V5h.5a.5.5 0 0 1 0 1h-2a.5.5 0 0 1 0-1zm0 3v-.5a.5.5 0 0 1 1 0V8h.5a.5.5 0 0 1 0 1h-2a.5.5 0 0 1 0-1zm0 3v-.5a.5.5 0 0 1 1 0v.5h.5a.5.5 0 0 1 0 1h-2a.5.5 0 0 1 0-1z"/>
</svg>
</a>
{% endif %}
{% if site.data.variables.show_slides_links and paper.slides %}
<a class="btn btn-outline-primary btn-sm d-print-none talk-btn" href="{{ paper.slides }}" data-bs-toggle="tooltip" data-bs-placement="bottom" data-bs-title="Slides">
<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-easel" viewBox="0 0 16 16">
    <path d="M8 0a.5.5 0 0 1 .473.337L9.046 2H14a1 1 0 0 1 1 1v7a1 1 0 0 1-1 1h-1.85l1.323 3.837a.5.5 0 1 1-.946.326L11.092 11H8.5v3a.5.5 0 0 1-1 0v-3H4.908l-1.435 4.163a.5.5 0 1 1-.946-.326L3.85 11H2a1 1 0 0 1-1-1V3a1 1 0 0 1 1-1h4.954L7.527.337A.5.5 0 0 1 8 0M2 3v7h12V3z"/>
</svg>
</a>
{% endif %}
</li>

{% endfor %}

</ul>

{% endif %}
