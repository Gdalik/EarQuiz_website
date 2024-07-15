---
layout: page
title:  "Annotations"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - ear training on equalization
    - learning frequencies
    - annotations
    - pink noise
    - peak normalization
    - audio file formats
---
#### Pink Noise

Pink noise is a kind of random noise which has equal energy in different octave ranges. It derives from white noise which
is a random signal with wide frequency range and equal power for each frequency. Since the number of frequencies in octave doubles
for each octave increase, the energy of white noise doubles in each higher octave as well, which is 3 dB/oct. boost. In other words, white noise
gives the *impression* of high-frequencies dominance.
In pink noise, the energy falls proportionally to frequency. I.e., it is similar to white noise, but with 3 dB/octave attenuation, starting from 1 Hz. 
This gives a much more even result from a human ear perspective, and the spectrum of pink noise is the closest one to an average music signal.

[< Back to "The Basic Training Method"][1]

#### Peak Normalization

Peak normalization of an audio file or its part is a linear change of its whole gain that makes the amplitude level of its (PCM) sample 
with the maximum amplitude equal to a certain value (in dB).

[< Back to "Checking Audio Playback"][2]<br />
[< Back to "Setting Volume Level"][3]

#### Supported Audio Formats

<a id="supported-audio-formats">Starting</a> from *version 0.1.7*, the application should flawlessly work with 
WAVE, AIFF, MP3, FLAC, and OGG files on all the supported platforms.</a>

[< Back to "The Basic Training Method"][1]<br />
[< Back to "Working with External Audio Files"][5]

[< Back to the Table of Contents]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/)

[1]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/basic-training-method/
[2]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/checking-audio-playback/
[3]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/adjusting-audio-system/#setting-volume-level
[4]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/converting-audio
[5]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/working-with-external-audio-files/
[6]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/choosing-audio-backend