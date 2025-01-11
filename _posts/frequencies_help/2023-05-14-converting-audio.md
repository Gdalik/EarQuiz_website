---
layout: page
title:  "Converting Audio Files"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - ear training on equalization
    - learning frequencies
    - converting audio files
    - resampling audio
    - export audio
---
The purpose of the in-app conversion tool is to convert audio files between different lossless formats, 
or to resample audio files. A user might need to downsample audio files with very high resolution (more than 48 kHz) 
to get sampling rates that are supported by his or her audio system, or just to reduce their size.

To convert audio file(s), first, select it/them. Second, choose the **File \| Convert Selected Files...** item from the main menu
or the same option from the right-click context menu of the **Playlist**.

In the opened dialog menu, you can choose the output format and the action to be done with sampling rate.
The available formats are WAV, AIFF and FLAC (since *version 0.1.8*).

The sampling rate options are the following:
- **Same as original**. The source file(s) are not resampled.
- **44100 Hz**. The sampling rate of the output file is set to 44.1 kHz, regardless of the source sampling rate.
- **48000 Hz**. The sampling rate of the output file is set to 48 kHz, regardless of the source sampling rate.
- **Auto choose 44100 Hz or 48000 Hz (downsample to multiple where original samplerate is higher)**. If the file sampling rate is 44.1 kHz
or the multiple of 44.1 kHz (88.2 kHz, 176.4 kHz, etc.), the output samplerate is set to 44.1 kHz. If the file sampling rate is 48 kHz
or the multiple of 48 kHz (96 kHz, 192 kHz, etc.), the output samplerate is set to 48 kHz.

When the original sampling rate of a file is changed, it is labeled as *Resampled* in the output filename.

After checking out or adjusting all the settings, press the **Convert** button to proceed.
When done, the new file(s) would be added to the **Playlist** after its/their source file(s).

[< Back to the Table of Contents]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/)