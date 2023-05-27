---
layout: page
title:  "Getting Started - Adjusting Audio System"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - Getting Started
    - ear training on equalization
    - learning frequencies
    - adjusting audio system
    - volume level
    - frequency response
    - frequency range
---

The flatter, the better. I mean frequency response of your whole playback system, of course.
If your audio path contains any tone controls, equalizers, or sound processors, which affect the spectrum of reproduced sound,
in most cases, they should be switched off or set flat, unless you know for sure that they compensate for the certain flaws. If you have the 
loudness compensation button on your playback preamp or receiver, it should be off as well.
<br/>

#### Setting Volume Level
The main idea for the volume is to set the comfortable level for the whole Learn/Test exercise cycle with the same audio stuff
and EQ pattern, without changing the loudness during or between separate examples. Please note that our frequency 
perception is heavily influenced by the sound level (for more details, see studies by Fletcher and Munson on this topic).
So, at this stage, it makes sense to adjust the volume to a comfortable medium loud level while you check the audio playback 
using pink noise and current EQ pattern. You may need to reconsider it later for different EQ patterns/settings or other audio sources.

There is a **Volume Slider** with the level indicator both in percents (slider value) and decibels (relative amplitude level), 
which can be accessed from the **Transport Panel**. The latter can be opened from various places, including the top-right corner 
of the **Audio Source** window and **View** menu of the main menu.

It would be ideal to calibrate the audio system once, and not to touch the volume levels during the whole training session since then.
There is no big problem with this when exercises are packaged into a finished and mastered audio product, like a complete CD.
Software lets us gain from flexibility and the possibility to create exercises with very different settings from any audio material on the fly. However, 
with in-app training we also run into a kind of compromise between sound quality, overall loudness and alignment of levels between 
exercises with different audio sources and settings.

As my priority is to achieve the best possible sound quality without clipping as a side effect of boosting frequencies,
I have decided to apply to every audio source of single-band exercise the preventive [peak normalization](#peak-normalization) with opposite number to current absolute value
of frequency gain.
For dual-band EQ patterns, I have added extra-headroom from 1 up to 3dB. 

So, there is an inverse relationship between equalization depth and peak normalization level (the more the frequency gain, 
the quieter the source before the equalization and vice-versa). 
The former can be set from ±1 to ±18 dB, whereas the latter can vary from -1 to -21 dB. Both values are displayed at the status bar
at the right-bottom side of the main window, which may be helpful when adjusting the volume level under different settings.

Please, also keep in mind that when listening to external audio files in the **Preview** mode, the tracks are played back as they are, 
without any preventive normalization applied.
As a result, commercially mastered and other tracks with maximized levels may sound too loud compared to the same tracks in the training 
(**Learn** and **Test**) modes. So, it is usually worth reducing the volume approximately by the absolute value of frequency gain 
before you switch from the training modes back to the **Preview** mode. For more convenient restoring of the
**Volume Slider** value for training, you may use the **Save Volume Level** and **Restore Volume Level** features, available from the **Volume Slider** 
right-click context menu or from the **Audio** menu of the main menu.

Considering all above-mentioned, I should acknowledge that I am still in search for the optimal and technically efficient
solution here, which would provide the best user experience without sacrificing quality.
<br />

#### Quick Checking Frequency Range and Response
To check out if your playback system reproduces the wide enough frequency range for our exercises, we will need
the special calibration test audio file. To generate it, simply select **File \| Make and Open Calibration Sine Waves File**
from the main menu. After having been created, the file "1kHz__10kHz__100Hz__15kHz__40Hz Sinus Tones.wav" will be added
to the **Playlist** and selected. To load it, you can just double-click on it or press the *Enter* key without changing the selection
(this will automatically set the relevant **Audio Source** mode and switch the application to the **Preview** mode as well; 
see details about [working with external audio files](#working-with-external-audio-files)).

The name of the file exactly reflects its content. There are five sinus tones with different frequencies, lasting 5 seconds
each, and separated with 1 second of silence from each other. All the tones have the equal amplitude, which is 20% of the highest
possible (approximately -14dB).

Here is the timeline table, to make it even clearer and easier to use:

| Frequency | Time (sec)  |
|:----------|:------------|
| 1 kHz     | 1&mdash;6   |
 | 10 kHz    | 7&mdash;12  |
| 100 Hz    | 13&mdash;18 |
| 15 kHz    | 19&mdash;24 |
| 40 Hz     | 25&mdash;30 |

You should be able to hear the first three tones (1 kHz, 10 kHz and 100 Hz) clearly. If they vary in loudness, it is not a problem
unless this difference is too big. If you cannot hear one or more of these, you have a serious issue with your playback system, which
must be resolved before going on. In case only the last two tones (15 kHz and 40 Hz) are barely audible or even inaudible, you can
proceed, but be aware that you may have difficulties hearing/identifying the low or the high extremes of the spectrum correspondingly. 
