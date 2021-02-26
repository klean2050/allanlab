---
title: "Kleanthis - Projects"
layout: textlay
excerpt: "Projects"
sitemap: false
permalink: /projects/
---

# Research Projects

My specialization lies in the fields of Signal Processing and Machine Learning Applications. Specifically, my research interests include:

* Audio, Music and Biomedical Signal Processing
* Behavioral Signals and Emotion Research
* Chaos, Fractals and Multifractal Signals
* Representation Learning and Autoencoders
* Multimodal Learning and Cross-Modal Retrieval

Here are some themes I currently work on, or worked in the past:

### Affective Analysis on EEG and Music

This is the topic of my Diploma Thesis, titled *Affective Analysis & Interpretation of Brain Responses to Music Stimuli*. Machine Learning has made overwhelming progress in modeling rational intelligence and the way humans perceive and act upon their environment. However, there are still many challenges in approaching emotion-driven intelligence, although it constitutes a fundamental aspect of human's perception and decision-making processes. The reason for this is that emotions are highly subjective, and thus really difficult to be labeled when expressed. There is though a growing interest in emotion tagging through physiological signals since those are induced without our active interference and thus depict more clearly the actual affective state. Such methods have been popular in designing Human-Computer Interfaces and also for medical purposes, among others for the detection of epilepsy and depression. The electroencephalogram (EEG) is the most widely researched neuronal signal and has been highly effective in detecting affective states. However, processing EEG signals and extracting useful features remain core challenges, since EEG, like most biological signals, is chaotic, nonlinear and incorporates a large amount of noise, both from the recording equipment and interfering physiological processes. In order to investigate the elicited affective characteristics, we choose to examine EEG signals from people listening to Music, since it has been shown that it greatly influences affective characteristics of the human mind.

* **Multifractal Analysis on EEG**: 
* **Deep Architectures for Emotion Recognition**:
* **EEG & Music Cross-Modal Learning**:

##### Related Publications:  
{% for publi in site.data.publist %}
{% if publi.project == "EEG" %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}
{% endfor %}

### Musical Instrument Classification

...
* **Augmentation Methods for Audio Mixtures**:
* **Modeling Audio Waveforms**:

##### Related Publications:  
{% for publi in site.data.publist %}
{% if publi.project == "IC" %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}
{% endfor %}
