---
layout: page
title:  "Making Training Audio Files"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - ear training on equalization
    - learning frequencies
    - making audio files
    - making exercises
    - export audio
    - Golden Ears
---
Learning and test exercises can be made in the form of audio file collections. 
The possible export formats are WAV, AIFF, MP3, FLAC, and OGG. So, you can use them either for self-studying or teaching
even without this application, just with any playback device or software which supports these common audio formats.

To make learning or test exercise audio file collection, select **File \| Make Learning Files...** or **File \| Make Test Files...**
from the main menu, correspondingly. Both options call the same dialog window, but with different **Type** setting selected, which 
can be changed afterward.

For the exercise files, the current audio source, EQ pattern and EQ settings will be used. The default parent output directory (**Exercise Folder**) is
*Documents/EarQuiz Frequencies/Exercises* in the current system user folder, but the dialog has an option which lets you change it.

By default, for each new exercise a new sub-folder with **Exercise Name** is created, and this name is used as the prefix
of each name of exported files, but you can switch off these options by unchecking the **Use as Folder Name** or 
**Use as Prefix of Filenames** settings. A default exercise name is generated automatically on each dialog window call, starting with
*Exercise1* and increasing the ending number (*Exercise2*, *Exercise3*, etc.) as needed so that the name would not repeat the name of an existing folder.

The number of learning audio files equals to the number of possible equalization options/combinations within a current EQ pattern.
The applied equalization (center frequency, boosted or cut) is indicated in the learning audio files' names.
The order of EQ bands is determined with the current settings of the **Controls \| EQ Bands Order in Learn Mode** menu of the
main menu. The examples are enumerated by default, but you can deactivate this option by unchecking the **Enumerate Learning Examples** option.

The number of test audio files in an exercise is always 10, and the examples are always enumerated, but you cannot get the answers from the filenames.

There is also a text file added to audio files. In case with learning exercises, *...Info.txt* includes the common information (audio source information, EQ pattern, EQ settings, peak normalization level, etc.)
The text file *...Answers.txt* of a test exercise collection in addition provides the right answers.

The sampling rate of exercise audio files is the same as the sampling rate of the audio source they are made from. The default bitrate of lossy formats (MP3 and OGG) is 320 kbps, 
but you can choose another one from the corresponding box.

After checking out or adjusting all the settings, press the **Make** button to proceed.

[< Back to the Table of Contents]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/)