---
layout: page
title:  "Getting Started - The Learn Mode"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - Getting Started
    - ear training on equalization
    - learning frequencies
    - learn mode
    - warm-up exercises
---
The basic way to activate the **Learn** mode is clicking the corresponding button on the main window or
by selecting **Controls \| Learn Mode** from the main menu. The keyboard shortcut for it is  **Ctrl+L** (on Windows or Linux) or **⌘L** (on macOS).<br />
![]({{ site.urlimg }}Frequencies_Help/LearnMode.png)<br />

The application will normalize the audio if needed. When you use an external audio file as a source, the program 
will read and crop it before that.
Then the playback of the first example will start automatically.

On each example playback, the corresponding EQ sliders' handles change their positions. And when the EQ is on, these sliders
are highlighted in green, and their labels show if the frequencies are boosted <span style="color:green; font-weight:bold">(+)</span>
or cut <span style="color:green; font-weight:bold">(-)</span>.

If you want to stop the playback of an example, use the **Stop** control/button or press the dot *(.)* key. To start playing the example once again, click 
the **Play** control/button or press the *Space* key. You can change the **EQ settings** between the playbacks. If you set another **Frequency Gain**,
the audio would be re-normalized.

By default, the EQ bands are played in the ascending order; if both boosting and cutting are available in the current
EQ pattern, each band is first boosted, then cut before proceeding to the next one. However, you can optionally change
this order to the descending or the shuffle one, selecting the appropriate option in **Controls \| EQ Bands Order in Learn Mode** menu
of the main menu. In boost & cut exercises, you can set the order with the sequence of all the bands boosted, and then 
all bands cut (or vice-versa), by selecting the option **All Bands Boosted, then All Bands Cut or VV** in the same menu.

To go to the next example, click the ![]({{ site.urlimg }}Frequencies_Help/next-example.png)**Next Example** control/button,
or press **Ctrl+Return** (on Windows and Linux) or **⌘+Return** (on macOS).

Alternatively, you can check the option ![]({{ site.urlimg }}Frequencies_Help/sequential-playback.png)**Sequential Playback (of Learning Examples)** 
in the **Controls** menu of the main menu or in the **Transport Panel**. In this case, you can start the playback once, and then
the application will make and play each next example automatically. With **Controls \| Loop Sequence (of EQ Bands)** unchecked,
it will stop after all possible EQ sliders' positions within the current EQ pattern have been gone through. Checking
this option will result in infinite loop until the playback is stopped.

Moving a slider handle (or two slider handles for dual-band patterns) will force the boost/cut of certain frequency band(s), and
this will become the first element of a sequence regardless of the EQ bands order set.

[< Back to the Table of Contents]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/)
