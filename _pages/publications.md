---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

## Preprints

{% assign preprints = site.publications | where: "category", "preprints" | sort: "date" | reverse %}

{% for paper in preprints %}
<div style="margin-bottom:1.5em;">

[{{ forloop.index }}]
<strong>{{ paper.authors }}</strong>.<br>

<em>{{ paper.title }}</em>.<br>

{{ paper.citation }}<br>

<a href="{{ paper.arxiv }}">arXiv</a>
·
<a href="{{ paper.pdf }}">PDF</a>

</div>
{% endfor %}

