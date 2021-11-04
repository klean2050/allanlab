---
title: "Kleanthis - Projects"
layout: textlay
excerpt: "Projects"
sitemap: false
permalink: /projects/
---

# Research Projects

Here are some themes I currently work on, or worked in the past:

### Affective Analysis on EEG and Music

Machine Learning has made overwhelming progress in modeling rational intelligence and the way humans perceive and act upon their environment. However, there are still many challenges in approaching emotion-driven intelligence, although it constitutes a fundamental aspect of human's perception. The reason for this is that emotions are highly subjective, and thus really difficult to be labeled when expressed. There is though a growing interest in emotion tagging through physiological signals since those are induced without our active interference and thus depict more clearly the actual affective state. The electroencephalogram (EEG) is the most widely researched signal of this kind. However, processing EEG signals and extracting useful features remain core challenges, since EEG, like most biological signals, incorporates a large amount of noise. In order to investigate the elicited affective characteristics, we choose to examine EEG from people listening to music, as it has been shown that it greatly influences affective operations in the human mind.

* **Multifractal Analysis on EEG**: The electroencephalogram is chaotic, nonlinear and incorporates a large amount of noise. The complex structure of such signals  has proven to be a serious barrier for traditional modeling methods. As a result, several nonlinear fractal methods have been proposed. Due to their complexity though, such signals do not always share the same structure over every time scale, hence the fractal characteristics may change dynamically or accordingly to the examined scale. Hence we propose the *Multiscale Fractal Dimension* and *Multifractal Detrended Fluctuation Analysis* to examine the EEG signals and determine emotional information buried in their fragmented structure.  

* **EEG & Music Cross-Modal Learning**: working on it :)  

Related Publications:  
{% for publi in site.data.publist %}
{% if publi.project == "EEG" %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}
{% endfor %}

### Musical Instrument Classification

...
* **Augmentation Methods for Audio Mixtures**: Most research in Instrument Classification deals with monophonic music, while efforts on polyphonic material mainly focus on predominant instrument recognition. Here we propose an approach for polyphonic music from predominantly monophonic data that involves performing data augmentation by mixing different audio segments. A variety of data augmentation techniques focusing on different sonic aspects, such as overlaying audio segments of the same genre, as well as pitch and tempo-based synchronization, are explored and we further investigate the usage of a combination of classifiers implementing the above methods. An ensemble of VGG-like classifiers yields state-of-the-art results for the IRMAS Dataset.

* **Modeling Audio Waveforms**: Audio Classification tasks are traditionally addressed through time-frequency representations of audio signals such as spectrograms. However, the emergence of deep neural networks as efficient feature extractors has enabled the direct use of audio signals for classification purposes. In this paper, we attempt to recognize musical instruments by only utilizing their raw waveforms. Various recurrent and convolutional architectures incorporating residual connections are examined and parameterized in order to build end-to-end classi-fiers with low computational cost and only minimal preprocessing. We obtain competitive classification scores and useful instrument-wise insight through the IRMAS Dataset, while maintaining a significantly reduced number of trainable parameters.

Related Publications:  
{% for publi in site.data.publist %}
{% if publi.project == "IC" %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}
{% endfor %}
