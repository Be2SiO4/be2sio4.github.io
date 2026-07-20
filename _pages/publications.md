---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

## Preprints

{% assign papers = site.publications | sort: "date" | reverse %}

{% for paper in papers %}

**[{{ forloop.index }}] {{ paper.authors }}.**  
{{ paper.title }}.  
{{ paper.citation }}  
[arXiv]({{ paper.arxiv }}) · [PDF]({{ paper.pdf }})

<br>

{% endfor %}
