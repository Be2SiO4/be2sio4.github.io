---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

## Preprints

{% assign preprints = site.publications | where: "category", "preprints" | sort: "date" | reverse %}

{% for paper in preprints %}

### [{{ paper.title }}]({{ paper.arxiv }})

{{ paper.authors }}

{{ paper.citation }}
&nbsp;  
[arXiv]({{ paper.arxiv }}) · [PDF]({{ paper.pdf }})

{% endfor %}
