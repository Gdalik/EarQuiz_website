---
layout: page
title:  "Getting Started - Working with External Audio Files"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - Getting Started
    - ear training on equalization
    - learning frequencies
    - playlist
    - loading audio files
---

There are different ways to load external audio into the software:
- Select **File \| Open Files...** from the main menu, or press **Ctrl+O** (on Windows) or 
**⌘O** (on macOS), or click on <span style="color:green; font-weight:bold">+</span> in the **Audio Source** window.
- Select **File \| Open Folder...** from the main menu.
- Drag & Drop files/folders to the **Playlist** from anywhere possible.

The methods above can be used both for locating audio files of [the supported formats]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/annotations/#supported-audio-formats) directly
or through playlists. Currently, parsing of M3U, M3U8, PLS and XSPF playlists is supported.

After adding audio files to the **Playlist**, you can load each of them in various ways.
If you haven't loaded any audio file before, in case you manually switch the **Audio Source** to the **Audio File (Playlist)** mode,
clicking the **Play** button or choosing **Controls \| Play** from the main menu will load and start playing the first track.
However, with **Shuffle Playback** option checked, a random audio file will be chosen. 

You can also load any track you want just by double-clicking on it or by selecting it and pressing *Enter*. This will switch the **Audio Source** to the 
**Audio File (Playlist)** mode automatically.

For further playlist navigation, you can use the ![]({{ site.urlimg }}Frequencies_Help/media-skip-backward_16.png) 
**Previous Track** / ![]({{ site.urlimg }}Frequencies_Help/media-skip-forward_16.png) **Next Track** player controls or similar buttons ![]({{ site.urlimg }}Frequencies_Help/arrows-right-and-left-filled-triangles.png) 
above the **Playlist**. 
When you are not in the **Preview** mode, the player skip controls/buttons are not available, though. In this case, if you want to go forward/backward
in the playlist, you can still use the navigation buttons above the **Playlist**. This will switch the program to the **Preview**
mode, whatever the current mode is. Any training process will be cancelled. Moreover, every change of an audio source resets the application to the **Preview** mode.
You can also manually activate the **Preview** mode by clicking the corresponding button on the main window or
by selecting **Controls \| Preview Mode** from the main menu. The keyboard shortcut for it is  **Ctrl+P** (on Windows) or **⌘P** (on macOS).<br /> 

![]({{ site.urlimg }}Frequencies_Help/PreviewMode.png)<br />

On the first switch to **Audio File (Playlist)**, 
the **Transport Panel** becomes visible automatically. Here we may take the most advantage of the latter.<br />

![]({{ site.urlimg }}Frequencies_Help/TransportPanel.png)<br />

One of the main purposes of the **Preview** mode is to let a user select and **trim** an audio track region for further training. The white vs
gray zone(s) of the audio timeline slider at the **Transport Panel** represent the trimmed region inside a whole audio track.
By default, each region starts at zero, and its length is equal to **Slice Length** (length of each future training example) multiplied by ten or by 
a smaller maximum number which can fit the length of a track. 

You can move left and right bounds of the region separately, and the whole region as well, by dragging the mouse cursor.
The start/end values can also be set with the corresponding spin boxes. Clicking on the <span style="color:blue; font-weight:bold">Start</span>
and the <span style="color:blue; font-weight:bold">End</span> buttons at the left sides of the spin boxes would set these values to
the current audio cursor position if possible, no matter if an audio file is playing or not. It may be pretty convenient to set the bounds
"on the fly" during the playback. The <span style="color:blue; font-weight:bold">[←</span> and the 
<span style="color:blue; font-weight:bold">→]</span> buttons at the right sides of the spin boxes can be used to set the starting
point to the beginning of a file, and to set the ending point to the end of a file, respectively.

The bounds' values of regions and the slice lengths are stored for each audio file on another file load or when the application
is about to be closed. When these audio files are loaded again (which is detected through hashing), these settings are restored.

Clicking the ![]({{ site.urlimg }}Frequencies_Help/clear.png)**Clear** button at the right of the start/end spin boxes resets the region bounds to default for newly loaded files, and
restores the previously saved values for already known ones.

The current **Playlist** and the latest audio source used are stored between sessions. However, I highly recommend 
saving the collections you would like to use repeatedly with **File \| Export Playlist...** options.

![]({{ site.urlimg }}Frequencies_Help/lightbulb.png)***Useful Tip***
 
*Before doing training exercises in the **Learn** and the **Test** modes, prepare your own collection of trimmed audio files, 
using the above-described application tools. Then uncheck the **Controls \| Start Playing After Loading Track in Preview Mode** 
option in the main menu if checked. [Adjust the volume level]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/adjusting-audio-system/#setting-volume-level) for your EQ Pattern and EQ Settings.
Load external audio files as audio sources for your exercises without playing them in the **Preview** mode. This will help you to
leave the volume knobs untouched as long as possible, while navigating through different audio sources/tracks.*