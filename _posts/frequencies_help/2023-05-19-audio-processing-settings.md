---
layout: page
title:  "Audio Processing Settings"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - audio processing settings
    - equalization
    - EQ
    - fade in
    - fade out
    - crossfade
---

In the *version 0.1.7*, the possibility to adjust the audio processing parameters of training 
examples has been introduced. This can be done from the dialog window
which is called by selecting **Audio | Audio Processing Settings** in the main menu.

![]({{ site.urlimg }}Frequencies_Help/audio-processing-settings.png)<br/>

The most important feature here, placed within the *Equalization Performance Settings* box, 
is the possibility to change the time proportion of **EQ Off** vs. **EQ On**
phases. It used to be hard-coded 
to <span style="color:gray; font-weight:bold">30%</span>/<span style="color:green; font-weight:bold">40%</span>/<span style="color:gray; font-weight:bold">30%</span> (<span style="color:gray; font-weight:bold">EQ Off</span>/<span style="color:green; font-weight:bold">EQ On</span>/<span style="color:gray; font-weight:bold">EQ Off</span> correspondingly).
And now a user can increase the length of the part where the equalizer is switched on by dragging the **<span style="color:green">EQ On</span> Time** slider
to the right, up to *100%*.

**EQ Always On In Test Mode** is another feature that has been added to the **Audio** menu in the main menu,
and it is closely related to the above-mentioned one. This makes sense when doing test exercises with either pink noise or
professionally mixed and mastered music tracks with polished spectral balance. When it is checked, the whole game becomes trickier, but it is closer to real-world situations. 
And the goal becomes not only to recognize the frequency bands that are boosted or cut, but also to develop the ability of 
detecting the issues that should be fixed, without reference to normal (non-processed) sound.

{% include alert warning='When **EQ Always On In Test Mode** is checked, **<span style="color:green">EQ On</span> Time** parameter 
inside the **Audio Processing Settings** window makes no effect on test exercises.' %}

The **Audio Processing Settings** window also contains a couple of more parameters.

The **EQ On↔︎Off Transition Time** parameter, which also refers to the *Equalization Performance Settings* group, is literally the length of the cross-fade between equalized and non-equalized parts of an example,
which prevents possible clicks at the transition places. A user can set a value between *1 ms* and *50 ms*, with the default one
being *35 ms*. The less, the faster; the bigger, the smoother.

And the **Example Fade In/Out Duration** setting has the default value of *5 ms*. You might want to set this to *zero* and do without
these fades, e.g., if you decide to [make learning files] [1] package, which you are going to play back continuously, without
pauses between examples within the sequence using your favorite media player. This is a way to do the learning exercises 
while enjoying the seamless, non-interrupted playback of a music track. Or a user might want to set this value to the maximum (*100 ms*) 
to get the smoothest possible starts and endings.

All the adjustable values in this window used to be hard-coded in the previous versions. Now that they have become the default settings, a user
can always bring them back by pressing the **Reset** button.

In order for the adjustments inside the **Audio Processing Settings** window to take effect, a user should press the **Apply** button.
If a training example is being played back, it will be stopped and reloaded.
Checking/unchecking the **EQ Always On In Test Mode** option has the same behavior, but it is applied immediately when in **Test** mode.

Adjusting any of the above-mentioned settings not only affects the training examples inside the program, but also changes these 
parameters for the [exported learning/test audio packages][1] correspondingly.

All these values are stored between application launch sessions.

[1]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/making-training-audio/

