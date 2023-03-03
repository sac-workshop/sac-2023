---
layout: default
title: Detailed call for papers and submission instructions
---

# Call for papers and submission instructions

The {{ site.data.variables.edition }} Conference on Selected Areas in Cryptography (SAC {{ site.data.variables.year }}) will take place at {{ site.data.variables.location_in_sentence }} in {{ site.data.variables.city }}, Canada on {{ site.data.variables.dates_conference }}, and will be preceded by the SAC Summer School on {{ site.data.variables.dates_school }}. {% if site.data.variables.iacr_in_cooperation_with %} SAC {{ site.data.variables.year }} is held in cooperation with the International Association for Cryptologic Research (IACR).{% endif %}

Authors are encouraged to submit original papers related to the following themes for SAC {{ site.data.variables.year }}. Note that the first three are traditional SAC areas; the fourth topic is the special focus for this year.

1. Design and analysis of symmetric key primitives and cryptosystems, including block and stream ciphers, hash functions, MAC algorithms, and authenticated encryption schemes.
2. Efficient implementations of symmetric and public key algorithms.
3. Mathematical and algorithmic aspects of applied cryptology.
4. {{ site.data.variables.fourth_topic }}.

SAC {{ site.data.variables.year }} also welcomes papers in any of the areas above with a focus on post-quantum cryptography.

{% if site.data.variables.proceedings_in_springer_lncs %}
The SAC {{ site.data.variables.year }} proceedings will be published by Springer in the Lecture Notes in Computer Science series.
{% endif %}

## Instructions for Authors

- Papers must be submitted electronically.  Late submissions, submissions by email, or hardcopy submissions will not be accepted.  {% if site.data.variables.url_submission %}{% else %}A submission link will be made available on the conference website prior to the submission deadline.{% endif %} 
- Submissions must be anonymous, with no author names, affiliations, acknowledgments or obvious references. 
- Papers must be typeset using LaTeX in the [LNCS style](https://www.springer.com/gp/computer-science/lncs/conference-proceedings-guidelines) with no alterations to font size or margins, with the exception of using `\pagestyle{plain}` to add page numbers. The main body of the paper must be at most 20 pages in length; including bibliography and clearly marked appendices, the total length must not exceed 30 pages. Program Committee members are not required to read appendices, so the paper should be intelligible without them.
- Papers must be written in English, and begin with a title, a short abstract, and a list of keywords. An introduction section should summarize the paper’s contributions at a level appropriate for a non-specialist reader.
- Submissions must be in PDF format.

{% if site.data.variables.url_submission %}
<div class="text-center"><a class="btn btn-primary" href="{{ site.data.variables.url_submission }}">Go to submission site</a></div>
<br>
{% endif %}

Submission implies the commitment of at least one of the authors to present the paper at the conference. The SAC {{ sites.data.variables.year }} Chairs reserve the right to withdraw papers from the proceedings that are not presented at the conference or for which the camera-ready post-proceedings version is not submitted by the deadline.

**Irregular submissions.**
SAC {{ sites.data.variables.year }} follows the IACR's Policy on Irregular Submissions. Submissions must not substantially duplicate work that any of the authors has published elsewhere or has submitted in parallel to a journal or any other conference/workshop that has proceedings. The SAC {{ sites.data.variables.year }} Chairs reserve the right to share information about submissions with other program committees or journal editors to detect parallel submissions. In addition, the SAC Chairs reserve the right to contact an author’s institution/corporation and/or other appropriate organizations if an irregular submission is detected. Submissions not meeting these guidelines risk rejection without consideration of their merits. For further details, please refer to the [IACR Policy on Irregular Submissions](https://www.iacr.org/docs/irregular.pdf).

**Conflicts of interest.**
SAC {{ sites.data.variables.year }} follows the IACR's Policy on Conflicts of Interest (COI). Authors, program committee members, and reviewers for SAC {{ sites.data.variables.year }} must adhere to the IACR Policy on Conflicts of Interest. Authors are requested to identify all members of the SAC {{ sites.data.variables.year }} Program Committee who have an automatic conflict of interest with the submission, and disclose it at the time of submission. It is the responsibility of all authors to ensure correct reporting of COI information. Submissions with incorrect or incomplete COI information may be rejected without consideration of their merits. For further details, please refer to the [IACR Policy on Conflicts of Interest](https://www.iacr.org/docs/conflicts.pdf).

**Code of conduct.**
SAC {{ sites.data.variables.year }} is committed to providing an experience free of harassment and discrimination, respecting the dignity of every participant. Participants who violate this code may be sanctioned and/or expelled from the event, at the discretion of the Chairs. Serious incidents may be referred to the IACR Ethics Committee for further possible action. Any action will only be taken with the consent of the affected party subject to applicable laws.

If you experience harassment or discriminatory behaviour at SAC {{ sites.data.variables.year }}, we encourage you to reach out to any of the SAC {{ sites.data.variables.year }} Chairs or the Chair of the SAC Board ({{ site.data.variables.sac_board_chair.name }} <[{{ site.data.variables.sac_board_chair.email }}](mailto:{{ site.data.variables.sac_board_chair.email }})>).

If you witness harassment or discriminatory behaviour, please consider intervening.

## Important dates

{% for d in site.data.dates %}
- <b>{{ d.name }}</b>: {{ d.date }} {{ d.time }} {% if d.url_convert_to_local_time %}• [Convert to local time]({{ d.url_convert_to_local_time }}){% endif %}
{%- endfor %}

## Program committee

{% if site.data.programcommittee.size > 0 %}

{% for member in site.data.programcommittee %}
- <b>{{ member.name }}</b>, {{ member.affiliation }}
{%- endfor %}

{% else %}

To be announced.

{% endif %}

## Stipends and Visas

Authors of accepted papers – particularly student authors – who are unable to attend the conference for financial reasons, may contact the organizers to apply for financial support. Stipends subject to availability of funds.

Conference attendees should refer to the [Government of Canada website](https://www.canada.ca/en/immigration-refugees-citizenship/services/visit-canada.html) for information about visa requirements to attend SAC {{ sites.data.variables.year }}.  Submitters who may require visas are encouraged to begin the process early, and in particular can contact the organizers after submission but prior to the notification deadline to request a letter of invitation.

## SAC Summer School

The SAC Summer School will be held prior to SAC, on {{ site.data.variables.dates_school }}, at {{ site.data.variables.location_in_sentence }}. The purpose of the SAC Summer School is to provide participants with an opportunity to gain in-depth knowledge of specific areas of cryptography related to the current SAC topics by bringing together world-class researchers who will give extended talks (half-day) in their areas of specialty. The SAC Summer School is open to all attendees, and may be of particular interest to students, postdocs, and other early-career researchers.

## SAC {{ sites.data.variables.year }} Organizing Committee

{% for organizer in site.data.organizers %}
- <b>{{ organizer.name }}</b>, {{ organizer.affiliation|join:", " }}
{%- endfor %}

General enquiries about SAC {{ sites.data.variables.year }}, including requests for invitation letters and questions about registration, should be sent to [{{ site.data.variables.organizer_email }}](mailto:{{ site.data.variables.organizer_email }}).
