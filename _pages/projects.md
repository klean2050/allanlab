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
* Multimodal Learning and Cross-Modal Retrieval

Here are some themes I currently work on, or worked in the past:

### Affective Analysis on EEG and Music

This is the topic of my Diploma Thesis, titled *Affective Analysis & Interpretation of Brain Responses to Music Stimuli*. Machine Learning has made overwhelming progress in modeling rational intelligence and the way humans perceive and act upon their environment. However, there are still many challenges in approaching emotion-driven intelligence, although it constitutes a fundamental aspect of human's perception and decision-making processes. The reason for this is that emotions are highly subjective, and thus really difficult to be labeled when expressed. There is though a growing interest in emotion tagging through physiological signals since those are induced without our active interference and thus depict more clearly the actual affective state. The electroencephalogram (EEG) is the most widely researched neuronal signal and has been highly effective in detecting affective states. However, processing EEG signals and extracting useful features remain core challenges, since EEG, like most biological signals, is chaotic, nonlinear and incorporates a large amount of noise, both from the recording equipment and interfering physiological processes. In order to investigate the elicited affective characteristics, we choose to examine EEG from people listening to music, as it has been shown that it greatly influences affective operations in the human mind.

* **Multifractal Analysis on EEG**: The electroencephalogram, like most biological signals, is chaotic, nonlinear and incorporates a large amount of noise. The complex structure of such signals  has proven to be a serious barrier for traditional modeling methods. As a result, several nonlinear fractal methods have been proposed. Due to their complexity though, such signals do not always share the same structure over every time scale, hence the fractal characteristics may change dynamically or accordingly to the examined scale. For this reason, we propose the *Multiscale Fractal Dimension* and *Multifractal Detrended Fluctuation Analysis* to examine the EEG signals and determine emotional information buried in their fragmented structure.  

* **Deep Architectures for Emotion Recognition**: working on it :)  

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
* **Augmentation Methods for Audio Mixtures**: Most research in Instrument Classification deals with monophonic music, while efforts on polyphonic material mainly focus on predominant instrument recognition. Here we propose an approach for polyphonic music from predominantly monophonic data that involves performing data augmentation by mixing different audio segments. A variety of data augmentation techniques focusing on different sonic aspects, such as overlaying audio segments of the same genre, as well as pitch and tempo-based synchronization, are explored and we further investigate the usage of a combination of classifiers implementing the above methods. An ensemble of VGG-like classifiers, trained on non-augmented, pitch-synchronized, tempo-synchronized and genre-similar excerpts, respectively, yields the best results for the IRMAS Dataset.

* **Modeling Audio Waveforms**: Sound Event Detection and Audio Classification tasks are traditionally addressed through time-frequency representations of audio signals such as spectrograms. However, the emergence of deep neural networks as efficient feature extractors has enabled the direct use of audio signals for classification purposes. In this paper, we attempt to recognize musical instruments in polyphonic audio by only feeding their raw waveforms into deep learning models. Various recurrent and convolutional architectures incorporating residual connections are examined and parameterized in order to build end-to-end classi-fiers with low computational cost and only minimal preprocessing. We obtain competitive classification scores and useful instrument-wise insight through the IRMAS test set, utilizing a parallel CNN-BiGRU model with multiple residual connections, while maintaining a significantly reduced number of trainable parameters.

Related Publications:  
{% for publi in site.data.publist %}
{% if publi.project == "IC" %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}
{% endfor %}
