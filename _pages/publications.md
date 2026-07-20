---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

## Preprints

{% assign preprints = site.publications | where: "category", "preprints" | sort: "date" | reverse %}

{% for paper in preprints %}
<div style="margin-bottom: 1.5em;">

[{{ forloop.index }}] **{{ paper.authors }}**.  
*{{ paper.title }}*.  
{{ paper.citation }}  
[arXiv]({{ paper.arxiv }}) · [PDF]({{ paper.pdf }})

</div>
{% endfor %}
