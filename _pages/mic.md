---
title: "News"
layout: textlay
excerpt: "Allan Lab at Leiden University."
sitemap: false
permalink: /mic.html
---

# Musical Instrument Classification

* **Augmentation Methods for Audio Mixtures**: Most research in Instrument Classification deals with monophonic music, while efforts on polyphonic material mainly focus on predominant instrument recognition. Here we propose an approach for polyphonic music from predominantly monophonic data that involves performing data augmentation by mixing different audio segments. A variety of data augmentation techniques focusing on different sonic aspects, such as overlaying audio segments of the same genre, as well as pitch and tempo-based synchronization, are explored and we further investigate the usage of a combination of classifiers implementing the above methods. An ensemble of VGG-like classifiers yields state-of-the-art results for the IRMAS Dataset.

* **Modeling Audio Waveforms**: Audio Classification tasks are traditionally addressed through time-frequency representations of audio signals such as spectrograms. However, the emergence of deep neural networks as efficient feature extractors has enabled the direct use of audio signals for classification purposes. In this paper, we attempt to recognize musical instruments by only utilizing their raw waveforms. Various recurrent and convolutional architectures incorporating residual connections are examined and parameterized in order to build end-to-end classi-fiers with low computational cost and only minimal preprocessing. We obtain competitive classification scores and useful instrument-wise insight through the IRMAS Dataset, while maintaining a significantly reduced number of trainable parameters.

Related Publications:  
{% for publi in site.data.publist %}
{% if publi.project == "IC" %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.venue }}</a>
{% endif %}
{% endfor %}
