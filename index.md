---
layout: home
title: Home
---

{:.fs-5}
Selected Areas in Cryptography (SAC) is Canada’s research conference on cryptography, held annually since 1994.

{:.fs-5}
The {{ site.data.variables.edition }} edition of SAC will take place at <b>{{ site.data.variables.location_in_sentence }}</b> in {{ site.data.variables.city }} Canada from <b>{{ site.data.variables.dates_conference }}</b>, and will be preceded by the <b>SAC Summer School</b> on <b>{{ site.data.variables.dates_school }}</b>.

<hr>

## Topics

There are four areas covered at each SAC conference. Three of the areas are permanent.

1. Design and analysis of symmetric key primitives and cryptosystems, including block and stream ciphers, hash function, MAC algorithms, cryptographic permutations, and authenticated encryption schemes;
2. Efficient implementations of symmetric and public key algorithms; and
3. Mathematical and algorithmic aspects of applied cryptology.

The special selected topic for SAC {{ site.data.variables.year }} is:

{:start="4"}
4. {{ site.data.variables.fourth_topic }}.

SAC {{ site.data.variables.year }} also welcomes papers in any of the areas above with a focus on post-quantum cryptography.

<hr>

## Conference Co-Chairs

{% for organizer in site.data.organizers %}
- <b>{{ organizer.name }}</b>, {{ organizer.affiliation|join:", " }}
{%- endfor %}

<hr>

## Important dates

{% for d in site.data.dates %}
- <b>{{ d.name }}</b>: {{ d.date }}
{%- endfor %}

## Virtual participation (updated on August 13, 2023)

Due to the delay of getting a Canada visa, we had to accomodate a number of talks virtually via Zoom at the last moment. If you plan to attend the conference virtually, an email should be sent to [{{ site.data.variables.organizer_email }}](mailto:{{ site.data.variables.organizer_email }}) for registration. 
