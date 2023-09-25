---
title: "Kleanthis - Publications"
layout: gridlay
excerpt: "Publications"
sitemap: false
permalink: /publications/
---

# Publications

For an updated list check my [Google Scholar](https://scholar.google.com/citations?user=mxLN1rUAAAAJ&hl=el) or [ResearchGate](https://www.researchgate.net/profile/Kleanthis_Avramidis).

{% for publi in site.data.publist %}

  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a><br />
  <em>{{ publi.authors }} </em><br />
  {{ publi.venue }}

{% endfor %}
