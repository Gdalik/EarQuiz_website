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
<a id="supported-audio-formats"> In general, the application works with WAVE, AIFF, MP3, FLAC and OGG files.</a>
All of them can be added to the **Playlist** and processed.

However, the support of the *playback* of different formats is dependent on the [current audio playback backend][6] (see the comparison in the table below).
Starting from *version 0.1.6*, you can choose between the **FFmpeg** (the default option) and the **Native** system backend by selecting
the corresponding option in the **Audio | Audio Playback Backend** menu of the main menu.

<br/>

| &nbsp; |                        FFmpeg                        |       Media Foundation<br/>(Native on Windows)       |         AVFoundation <br/>(Native on macOS)          |           GStreamer <br/>(Native on Linux)           |
|:------:|:----------------------------------------------------:|:----------------------------------------------------:|:----------------------------------------------------:|:----------------------------------------------------:|
 |  WAVE  | <span style="color:green; font-weight:bold">✓</span> | <span style="color:green; font-weight:bold">✓</span> | <span style="color:green; font-weight:bold">✓</span> | <span style="color:green; font-weight:bold">✓</span> |
|  AIFF  | <span style="color:green; font-weight:bold">✓</span> |  <span style="color:red; font-weight:bold">✗</span>  | <span style="color:green; font-weight:bold">✓</span> | <span style="color:green; font-weight:bold">✓</span> |
|  MP3   | <span style="color:green; font-weight:bold">✓</span> | <span style="color:green; font-weight:bold">✓</span> | <span style="color:green; font-weight:bold">✓</span> | <span style="color:green; font-weight:bold">✓</span> |
  |  FLAC  | <span style="color:green; font-weight:bold">✓</span> | <span style="color:green; font-weight:bold">✓</span> | <span style="color:gray; font-weight:bold">✓</span>* | <span style="color:green; font-weight:bold">✓</span> |
|  OGG   | <span style="color:green; font-weight:bold">✓</span> |  <span style="color:red; font-weight:bold">✗</span>  |  <span style="color:red; font-weight:bold">✗</span>  | <span style="color:green; font-weight:bold">✓</span> |

*\*AVFoundation which is used natively on macOS, has a known issue with 
incorrect FLAC files' playback position, which may occur when starting playing from a non-zero position.*<br/>

<br/>

All backends support the playback of WAVE, MP3 and FLAC files. 

If you try to load a file of a format which is not supported by the current backend, you will get an error message
with option to proceed with [conversion to another (WAVE or AIFF) format](https://earquiz.org/manuals/earquiz-frequencies-help/converting-audio/). 

So, when you encounter any issue with playing back files of a certain format, you have two options:
- Change the **Audio Playback Backend**. This will require restarting the application.
- Use the in-app audio conversion tool, selecting these files and choosing 
**File | Convert Selected Files...** from the main menu or the similar option from the right-click context menu of the **Playlist**.

[< Back to "The Basic Training Method"][1]<br />
[< Back to "Working with External Audio Files"][5]

[< Back to the Table of Contents]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/)

[1]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/basic-training-method/
[2]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/checking-audio-playback/
[3]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/adjusting-audio-system/#setting-volume-level
[4]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/converting-audio
[5]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/working-with-external-audio-files/
[6]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/choosing-audio-backend