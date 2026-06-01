
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
---------------------

{% include base_path %}

<div style="margin-bottom:20px;">

This page presents a selection of my scientific publications and industry contributions related to Central Bank Digital Currencies (CBDCs), digital identity, secure payment systems, applied cryptography, privacy-preserving technologies, and fraud detection.

For a complete and up-to-date publication record, please visit my <a href="https://scholar.google.com/citations?user=fh9JvWgAAAAJ&hl=fr&oi=ao"><strong>Google Scholar</strong></a>
or <a href="https://orcid.org/0009-0007-9655-2641"><strong>ORCID</strong></a>
profiles.

</div>

<hr>

<h2>Journal Articles</h2>

{% assign journals = site.publications | where: "pubtype", "journal" %}
{% if journals.size > 0 %}
{% for post in journals reversed %}
{% include archive-single-cv.html %}
{% endfor %}
{% endif %}

<h2>Conference Papers</h2>

{% assign proceedings = site.publications | where: "pubtype", "proceeding" %}
{% if proceedings.size > 0 %}
{% for post in proceedings reversed %}
{% include archive-single-cv.html %}
{% endfor %}
{% endif %}

<h2>PhD Thesis</h2>

{% assign theses = site.publications | where: "pubtype", "thesis" %}
{% if theses.size > 0 %}
{% for post in theses reversed %}
{% include archive-single-cv.html %}
{% endfor %}
{% endif %}

<h2>Industry Reports & White Papers</h2>

{% assign reports = site.publications | where: "pubtype", "report" %}
{% if reports.size > 0 %}
{% for post in reports reversed %}
{% include archive-single-cv.html %}
{% endfor %}
{% endif %}

<h2>Preprints</h2>

{% assign preprints = site.publications | where: "pubtype", "preprint" %}
{% if preprints.size > 0 %}
{% for post in preprints reversed %}
{% include archive-single-cv.html %}
{% endfor %}
{% endif %}
