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
  ![Conference](http://img.shields.io/badge/2023-ICASSP-4b44ce.svg) <em>{{ publi.authors | replace: "Kleanthis Avramidis", "<strong>Kleanthis Avramidis</strong>" }} </em><br />
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a><br />
  {{ publi.venue }}
{% endfor %}
