---
layout: default
title: About
---

# About SAC

The [Selected Areas in Cryptography (SAC) conference series](http://sacworkshop.org/) was initiated in 1994, when the first event was held at Queen’s University in Kingston. The SAC conference has been held annually since 1994 in various Canadian locations.  The conference series is maintained by the [SAC Board](https://sacworkshop.org/contact.html).

{% if site.data.variables.iacr_in_cooperation_with %}
<div class="float-end">
  <img src="images/iacr.png" style="max-height: 60px;" alt="IACR logo">
</div>

SAC {{ site.data.variables.year }} is held in co-operation with the <a href="https://iacr.org">International Association for Cryptologic Research (IACR)</a>, which is the leading scholarly organization for cryptographic research.
{% endif %}

<div style="clear: both;"></div>

{% if site.data.variables.proceedings_in_springer_lncs %}
<div class="float-end">
  <img src="images/springer_lncs.png" style="max-height: 60px;" alt="Springer LNCS logo">
</div>

The SAC proceedings are published by Springer in the <a href="https://www.springer.com/gp/computer-science/lncs">Lecture Notes in Computer Science series</a>.
{% endif %}

<div style="clear: both;"></div>

<hr>

## SAC {{ site.data.variables.year }} Organizers

{% for organizer in site.data.organizers %}
#### {{ organizer.name }} – {{ organizer.role}}

<div class="float-start">
  <img src="{{ organizer.image|e }}" alt="{{ organizer.name|e }}">&nbsp;&nbsp;&nbsp;
</div>

{% for affiliation_line in organizer.affiliation -%}
{{ affiliation_line }}<br>
{%- endfor -%}
[{{ organizer.url }}]({{ organizer.url }})

<div style="clear: both;">&nbsp;</div>

{% endfor %}

<hr>

## Program committee

{% if site.data.programcommittee.size > 0 %}

{% for member in site.data.programcommittee %}
- <b>{{ member.name }}</b>, {{ member.affiliation }}
{%- endfor %}

{% else %}

To be announced.

{% endif %}