---
layout: page
title:  "Getting Started - Choosing Audio Playback Backend"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - Getting Started
    - audio backend
    - FFmpeg
    - Windows Media Foundation
    - AVFoundation
    - GStreamer
---

{% include alert info='This option was deprecated in *version 0.1.7*. The bug in Qt6/PyQt6 
library that caused deadlock when using *FFmpeg* backend and led to the application hanging was fixed.
Now, *FFmpeg* is used as a single possible framework for playing all the supported audio formats on all the supported platforms.' %}

***Version 0.1.6***

This option was introduced in *version 0.1.6* along with the support of *FFmpeg*, which has now been used by default. 
Before that, the native system backend (*Windows Media Foundation* on Windows, and *AVFoundation* on macOS)
had been the only option. The Linux version, which also appeared in this release, uses *GStreamer* as the underlying framework.
To switch between *FFmpeg* and the native audio playback backend, just select the corresponding option in **Audio | Audio Playback Backend**
menu of the main menu. The program restart is required for the changes to take effect, so the dialog window, asking for your
permission to do that, will appear.

The main advantage of *FFmpeg* is that it is cross-platform and overcomes some limitations
of native multimedia backends. It lets the program play audio files of all the [audio formats][1]
which can be added to the **Playlist** without the need to use the in-app [conversion tool][2]. The playback position timing
also tends to be more exact, especially comparing to *AVFoundation* handling of FLAC files. On Ubuntu (Linux), *FFmpeg* showed 
more stable performance than *GStreamer* when testing the application manually. 

However, the app's GUI (including the audio playback part) is built upon the *PyQt6* framework, with all its strengths and pitfalls.
Since QT introduced the *FFmpeg* support as the technology preview, not all the stability issues seem to be fixed yet.
While the manual tests showed the stable performance on Windows and Linux, on macOS, it sometimes leads to the program hanging 
or freezing when a new audio file is being loaded. So, when the crashless performance is the priority, switching to the native backend on macOS
is recommended.

[1]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/annotations/#supported-audio-formats
[2]: {{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/converting-audio


[< Back to the Table of Contents]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/)