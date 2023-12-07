---
title: "Kleanthis - Publications"
layout: gridlay
excerpt: "Publications"
sitemap: false
permalink: /publications/
---

# Publications

For an updated list check my [Google Scholar](https://scholar.google.com/citations?user=mxLN1rUAAAAJ&hl=el).

{% for publi in site.data.publist %}
  {% if publi.link.doi %} <a href="{{ publi.link.doi }}"><img src="http://img.shields.io/badge/{{ publi.badge }}-c41e3a" height="23" /></a> {% else %} <img src="http://img.shields.io/badge/{{ publi.badge }}-c41e3a" height="23" /> {% endif %}
  {% if publi.link.code %} <a href="{{ publi.link.code }}"><img src="http://img.shields.io/badge/code-390eb0" height="23" /></a> {% endif %}
  <div style="font-size: 17px; margin-top: -10px;">
  <em>{{ publi.authors | replace: "Kleanthis Avramidis", "<strong>Kleanthis Avramidis</strong>" }} </em><br />
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a><br />
  {{ publi.venue }}
  </div>
{% endfor %}
