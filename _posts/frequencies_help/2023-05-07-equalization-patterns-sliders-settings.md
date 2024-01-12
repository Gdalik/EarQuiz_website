---
layout: page
title:  "Getting Started - Equalization: Patterns, Sliders and Settings"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - Getting Started
    - eq patterns
    - eq sliders
    - eq setttings
    - filter bandwidth
    - filter Q
    - filter gain
---

#### Equalization Patterns
**EQ Pattern** is a core of each exercise, as it defines:
- the range of frequency options;
- default **EQ Settings** (Frequency Gain and Bandwidth/Q factor of filters);
- the type of **Equalizer**: 1-octave (10-band) or 1/3-octave (30-band);
- if the frequencies would be boosted or cut, or both options;
- if one or two frequency bands would be treated at once;
- for dual-band presets: the minimal range between altered frequency bands.

There are 15 presets with increasing difficulty: from boosting a single 1-octave band within a limited frequency range (lows, mids, highs separately)
to boosting or cutting two 1/3-octave bands simultaneously in the full range. 
You can choose any pattern from the list or skip forward with the <span style="color:blue; font-weight:bold">></span> 
(**Next Equalization Pattern**) button. This can be made silently (without triggering other actions) in the **Preview** mode, 
unlike in the **Learn** or the **Test** modes, where it resets the exercises and their playback.

The current EQ pattern is stored between sessions.
<br />

#### Equalization Sliders
**EQ Sliders** are the main input controllers for the training (**Learn** and **Test**) modes. The numbers below each of them
represent the central frequencies of corresponding frequency bands. And the positions of sliders' handles determine the boost or cut
of particular bands, whether real (while learning) or guessed (while testing).

However, in the **Learn**
mode one may need to manually trigger them only to force the boost/cut of specific frequencies in the following example,
since this is done automatically otherwise. In the **Test** mode a user enters his or her answers pushing the 
appropriate sliders' handles up or down.

The frequency range of the current EQ Pattern determines the range of available/enabled sliders when the app is ready for
the corresponding input. The 25Hz and the 20kHz sliders of the 30-Band EQ are permanently disabled, since these frequencies are 
at the boundaries of our perception and most systems' reproduction.

The initial positions of sliders' handles depend on the current EQ Pattern. If frequency bands are to be boosted, they are
at the bottom of the sliders. If frequency bands are to be cut, they are at the top of the sliders. When both options
are possible, the handles are at the vertical center.

With *single-band* patterns, the input is accepted when a user changes the position of a slider handle. There is no way to
change the mind within the example here.

With *dual-band* patterns, the input is accepted when the position of two sliders' handles
is changed. After a user has dragged or clicked on a first slider, one or more adjacent sliders are disabled.
This is because the option to simultaneously alter two frequency bands, that are too close to each other, is intentionally
avoided, as it would become a kind of "mind game" otherwise. While the user hasn't chosen a second slider, he or she can
return the first one to its initial state and reconsider the input.
<br />

#### Equalization Settings
You can open the **EQ Settings** by clicking the button with ![]({{ site.urlimg }}Frequencies_Help/settings_16.png) 
gear icon in the top-right corner of the EQ or by selecting **View \| EQ Settings** from the main menu.
They consist of two parameters: 
1. *Frequency Gain*, that determines an amount by which the center frequency of filter is boosted or cut.
2. *Bandwidth*/*Q factor*, that are used to set the width of boosted or cut frequency band.

Here is a filter frequency response scheme:

![]({{ site.urlimg }}Frequencies_Help/BellFilterScheme.png)

This type of filter is called *peaking* or *bell* band-pass filter.
Center frequency (f<sub>0</sub>) which is determined by the choice of an EQ Slider, is the most altered (boosted or cut) 
point within a frequency band.
To measure how wide or narrow the whole band is, we need two symmetrical points on the left (f<sub>1</sub>) and 
on the right (f<sub>2</sub>) side of this peak, which have the 3dB roll-off (50% drop in power/energy).

The absolute bandwidth (BW) in Hz is simply the difference between the highest and the lowest frequencies:

![]({{ site.urlimg }}Frequencies_Help/BW_form.png)
<br />

But our perception is not linear. The same music intervals will contain different number of Hz in different spectral ranges.
An absolute difference in Hz doubles with each increase of 1 octave.
That is to say, there is an octave between 50 and 100 Hz, 100 and 200 Hz, 200 and 400 Hz, 400 and 800 Hz, etc.
So, for our ears, the *ratio* between frequencies (f<sub>2</sub>/f<sub>1</sub>) matters much more than their absolute difference. 
This is why bandwidth of filters is also measured in octaves.

To calculate the difference in octaves between f<sub>1</sub> and f<sub>2</sub>, means to detect how many times we should multiply
f<sub>1</sub> by 2 to get f<sub>2</sub>. If we translate this into algebraic expression, we get the following formula:

![]({{ site.urlimg }}Frequencies_Help/BWoct_form.png)
<br />

In our case, we deal with 1-octave and narrower bands, that's why we have BW values between 0 and 1.

Even more often than BW, we encounter the *Q factor* (abbrev. from *Quality factor*) as a filter parameter. Though used interchangeably often, 
they are not the same. In fact, they have inverse correlation: the bigger the Q, the narrower the band; the wider the band, 
the smaller the Q. If we know the absolute BW in Hz and the center frequency of a filter, the Q is easily calculated:

![]({{ site.urlimg }}Frequencies_Help/Q_from_BW_form1.png)
<br />

But as we mostly deal with relative BW in octaves, we might want to know, how to convert them to those weird Q numbers.
This formula is a bit more complicated:

![]({{ site.urlimg }}Frequencies_Help/Q_from_BW_form2.png)<br />
where N is number of octaves.

Enough with algebra and formulas here. The one that converts Q factor to BW in octaves is rather big, by the way.

For *Bandwidth* options, I have used the values which can easily be thought of as music (tempered-scale) intervals:

| Bandwidth | Q      | Interval |
|:----------|:-------|:---------|
 |1 Octave | ~1.41  | Octave   |
| 3/4 Octave| ~1.9   | Major 6th |
| 2/3 Octave| ~2.14  | Minor 6th |
| 1/2 Octave | ~2.87  | Tritone  |
| 1/3 Octave | ~4.32  | Major 3d |
| 1/4 Octave | ~5.76  | Minor 3d |
| 1/6 Octave | ~8.65  | Major 2nd |

In general, the narrower/steeper filter curve, the more accurately and precisely it works.
The wider band, conversely, affects more frequencies and makes equalization more prominent, but less exact.
With too high Q factor, the situation,
when there is no audible content in particular part of spectrum, is more likely. With too low one, the boundaries
between frequency bands may become blurred.

For presets with 10-band EQ I have set the default bandwidth to 1 octave with ±12dB gain, and for those with 30-band EQ I have used
the 1/3-octave value with ±15dB gain.

You can set your custom options in the **Preview** mode or in the **Learn** mode between playbacks of examples. The app
will re-normalize your audio according to current Frequency Gain and EQ pattern. Clicking the **Reset** button restores 
default EQ pattern settings.

If you want to use the same settings across various EQ patterns, you can **Lock** them with the corresponding button.
For example, you have become confident with all the patterns, and you want to boost your proficiency. In this case,
while going through the same patterns, 
you can try lowering the frequency gain value, and challenge your ears to hear the subtler and subtler equalization.

When locked, this state and values themselves are stored between sessions.

[< Back to the Table of Contents]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/)
