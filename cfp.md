---
layout: default
title: Call for papers
---

# Call for papers

Authors are encouraged to submit original papers related to the following themes for Selected Areas in Cryptography (SAC) {{ site.data.variables.year }}. Note that the first three are traditional SAC areas; the fourth topic is the special focus for this year.

1. Design and analysis of symmetric key primitives and cryptosystems, including block and stream ciphers, hash functions, MAC algorithms, and authenticated encryption schemes.
2. Efficient implementations of symmetric and public key algorithms.
3. Mathematical and algorithmic aspects of applied cryptology.
4. {{ site.data.variables.fourth_topic }}.

SAC {{ site.data.variables.year }} also welcomes papers in any of the areas above with a focus on post-quantum cryptography.

#Download the detailed call for papers (PDF).

<div class="text-center"><a class="btn btn-primary" href="cfp-detailed.html">Submission instructions</a></div>

<br>

## Important dates

{% for d in site.data.dates %}
- <b>{{ d.name }}</b>: {{ d.date }} {{ d.time }}
{%- endfor %}
