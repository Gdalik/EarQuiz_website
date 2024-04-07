---
layout: page
title:  "Application Data and Settings"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - ear training on equalization
    - learning frequencies
    - application data
    - application settings
---
I tried to make the program store all its data and settings in one place, without leaving
a lot of scattered garbage on disk or in registry (on Windows). On macOS, the (parent) data/settings directory is *Library/Application Support/EarQuiz/Frequencies* 
under current system's user folder. On Windows, it is located in *EarQuiz/Frequencies* folder under the current user's 
*Application Data* folder. And the path on Linux is *.config/EarQuiz/Frequencies* in a user's home directory.
Therefore, by manually removing it or some parts of it, you can reset the corresponding settings to defaults.
Moreover, automatic clean-up of all the application data during the uninstallation process (which is often not desirable) becomes unnecessary.

The *config.ini* file contains the program settings and states, including checked/unchecked options, windows'/panels' sizes, placements and
visibilities, last used audio source and EQ pattern, locked EQ settings, etc.

The audio tracks' paths of the current **Playlist** are stored in *current.m3u8* file inside the *Playlists* sub-folder.

The trimmed ranges (starting and ending points) and the slice length values of audio files are stored inside the *SourceRangeLib* sub-folder.
Each loaded audio file is hashed, and the data about each audio file is saved as a separate JSON format file with 
the name of md5 hash-sum of the corresponding audio file and the **.afab (Audio File A-B)* extension. You can also see the audio file name
inside each of these JSON data files. Hashing big files is not a very fast process, but this method allows the program to identify files in a path-independent
and platform-independent way. That said, you can even transfer these  **.afab* files
to a similar folder on another computer, and the copy of the application, running on that machine, would be able to apply these
settings/data to the identical copies of your audio files.

[< Back to the Table of Contents]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/)