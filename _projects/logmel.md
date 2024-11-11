---
layout: page
title: APCCAS 2024
description: log mel-spectrogram implementation
img: assets/img/logmel.jpg
importance: 2
category: work
related_publications: false
---

#### A 250.3mW Versatile Sound Feature Extractor Using 1024-Point FFT 64-ch LogMel Filter in 40nm CMOS
###### [Akiho Kawada](https://akiho-kawada.github.io/), [Kenji Kobayashi](https://www.kenjikoba.com/), Jaewon Shin, [Rei Sumikawa](https://jp.linkedin.com/in/rei-sumikawa-2b083625b), [Mototsugu Hamada](https://ieeexplore.ieee.org/author/37088514166), [Atsutake Kosuge](https://sites.google.com/view/atsutakekosuge-eng/home)

<br>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/logmel_overview.png" title="proposed method overview"  class="img-fluid rounded z-depth-1" style="height: 50px" %}
    </div>
</div>



<br>

##### _Abstract_
A 250.3µW always-on sound feature extractor that facilitates general-purpose sound recognition AI processing encompassing 35-word voice command recognition, environmental sound recognition, and musical instrument recognition is developed.

Conventionally, approximated mel- frequency cepstrum coefficients (MFCC) feature extractors composed of a limited number of FFT samples (256 points), and filter channels (10 channels) are utilized for energy reduction; however, their applicability is restricted to wake-up word recognition resulting in high NRE costs.

To overcome these challenges, we developed a LogMel filter feature extractor employing a 1024-point FFT and 64-channel Mel filter bank, which enables versatile applications across a diverse range of sound recognition tasks including 35-word voice command recognition. 
To minimize circuit area and power consumption, three techniques are employed: <br>
(a) radix-22 single-path delay feedback (R22SDF) which uses serial FFT processing for circuit area reduction, <br>
(b) zero-skipping Mel filter bank for a 1/25x circuit area reduction by storing and accumulating only non- zero elements, and <br>
(c) Log LUT, an LUT approximation to reduce the number of cycles by a factor of 20 compared with the CORDIC implementation. <br>

Designed and implemented in a 40nm CMOS process, the proposed extractor demonstrates a power efficiency of 14.9nJ/frame/word for a 35-word voice command recognition task, showcasing a 1.1× improvement in power efficiency and a 17.5 × increase in the number of recognizable voice commands compared to state-of-the-art KWS-specific simplified MFCC audio extraction circuits.

<br>

##### _Authors' Preprint_
[pdf](https://drive.google.com/file/d/1nyJjVpdPvio8WRDi3DD_--86FPmZVhed/view?usp=drive_link)

<br>

##### _Presentation PDF_
[presentation](https://drive.google.com/file/d/1Qc6F8eWOVGl_zb4NhoU9x78hLvn5m4xv/view?usp=sharing)

