---
layout: page
title:  "The Basic Training Method"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - ear training on equalization
    - learning frequencies
---

The overall training process involves ongoing learning and testing yourself.
Both learning and test exercises consist of audio samples, which we will call *examples*. Each example is a 10-30 
seconds' long chunk of either **[pink noise][1]** (generated on each application launch) or **music**.  
Technically, any external audio file of a [supported format][2], stored locally on your device, can be used instead for the latter.
So, you could further experiment with recordings of speech, different sounds, natural or synthetic noises, 
whatever you have in your audio collection.

The method behind every example is fairly simple. It begins normally, with no spectral changes. After several seconds, 
the octave or 1/3-octave graphic equalizer (EQ) which boosts or cuts the amplitude of one or two frequency bands, is switched on 
automatically. After some more seconds, the EQ is switched off again, and the sound is returned to its normal 
(non-equalized) state.

![]({{ site.urlimg }}Frequencies_Help/Drill_structure.png)

*Note: The default proportion of equalized part length versus sum length of non-equalized ones is hard-coded at 40/60 per cent.
Therefore, if we have 10 seconds length example, this would be: 3sec **EQ Off**, 4sec **EQ On** and 
3sec **EQ Off** respectively. It used to be hard-coded, but in the version 0.1.7 the option to adjust this setting as well as 
some other audio processing parameters has been introduced. [See details here][4].*

Regardless of the audio source material and the EQ settings, the recommended approach remains the same.
- First, you **learn** and warm-up by listening to examples, trying to [memorize and internalize][3] 
the sound of different frequency ranges. <br /> *Don't be scared; relax, listen, watch the
highlighted sliders and frequency values on the screen, and let your brains do the job ;-)!*
- Second, you take a **test** which is nothing but a sequence of ten similar examples with randomly chosen frequency values 
and boost/cut options (where available), which you guess, and get a score to track your progress.

[< Back to the Table of Contents]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/)

[1]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/annotations/#pink-noise
[2]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/annotations/#supported-audio-formats
[3]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/memorizing-frequencies
[4]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/audio-processing-settings