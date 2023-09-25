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
  <em>{{ publi.authors }} </em><br />
  {% assign authors_array = publi.authors | split: ', ' %}
  {% for author in authors_array %}
    {% if author contains "Kleanthis Avramidis" %}
      <em><strong>{{ author }}</strong></em>
    {% else %}
      <em>{{ author }}</em>
    {% endif %}{% unless forloop.last %}, {% endunless %}
  {% endfor %}
  
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a><br />
  {{ publi.venue }}

{% endfor %}
