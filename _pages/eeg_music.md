---
title: "News"
layout: textlay
excerpt: "Allan Lab at Leiden University."
sitemap: false
permalink: /eeg_music.html
---

# :brain: Musical Emotions and EEG Signals

Machine Learning has made overwhelming progress in modeling rational intelligence and the way humans perceive and act upon their environment. However, there are still many challenges in approaching emotion-driven intelligence, although it constitutes a fundamental aspect of human's perception. The reason for this is that emotions are highly subjective, and thus really difficult to be labeled when expressed. There is though a growing interest in emotion tagging through physiological signals since those are induced without our active interference and thus depict more clearly the actual affective state. The electroencephalogram (EEG) is the most widely researched signal of this kind. However, processing EEG signals and extracting useful features remain core challenges, since EEG, like most biological signals, incorporates a large amount of noise. In order to investigate the elicited affective characteristics, we choose to examine EEG from people listening to music, as it greatly influences affective operations in the human mind.

* **Multifractal Analysis on EEG**: The electroencephalogram is chaotic, nonlinear and incorporates a large amount of noise. The complex structure of such signals  has proven to be a serious barrier for traditional modeling methods. As a result, several nonlinear fractal methods have been proposed. Due to their complexity though, such signals do not always share the same structure over every time scale, hence the fractal characteristics may change dynamically or accordingly to the examined scale. Hence we propose the *Multiscale Fractal Dimension* and *Multifractal Detrended Fluctuation Analysis* to examine the EEG signals and determine emotional information buried in their fragmented structure.  

* **EEG & Music Cross-Modal Learning**: The study of Music Cognition and neural responses to music has been invaluable in understanding human emotions. Brain signals, though, manifest a highly complex structure that makes processing and retrieving meaningful features challenging, particularly of abstract constructs like affect. In this paper we extract efficient, personalized affective representations from EEG signals during music listening. To this end, we employ music signals as a supervisory modality to EEG, aiming to project their semantic correspondence onto a common representation space. The experimental findings show the potential of enhancing neuronal data through stimulus information for recognition purposes and yield insights into the distribution and temporal variance of music-induced affective features.

Related Software:

<div class="gh-card gh-medium" data-repo="aranscope/github-cards"></div>

Related Publications:  
{% for publi in site.data.publist %}
{% if publi.project == "EEG" %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.venue }}</a>
{% endif %}
{% endfor %}
