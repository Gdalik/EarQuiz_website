---
layout: page
title:  "Creating, Editing and Saving Playlists"
breadcrumb: true
categories:
    - manuals
    - earquiz-frequencies-help
tags:
    - EarQuiz Help
    - ear training on equalization
    - learning frequencies
    - creating playlist
    - editing playlist
    - exporting playlist
---
Basically, within the software, the single playlist (and the corresponding **Playlist** widget inside the **Audio Source** window) 
is used. You can add the tracks you are going to use as audio sources
for your exercises to it, reorder them and remove them. The **Playlist** widget is a table with 3 columns: **Filename**, **Duration** and **Folder Path**. 
The playlist contents are saved and restored on each program startup
unless cancelled by user. You can also export them to separate playlist files, which is highly recommended every time 
you make a collection of tracks that would be reused in the future.

{% include alert warning='Whether the application reloads the internal playlist or imports data from external playlist files, only the existing audio files of
the supported formats are added as items.' %}
 
#### Adding and Removing Tracks
Different ways can be used to add audio tracks into the application **Playlist**:
- Select **File \| Open Files...** from the main menu, or press **Ctrl+O** (on Windows) or 
**⌘O** (on macOS), or click on the <span style="color:green; font-weight:bold">+</span> button in the **Audio Source** window. 
Then choose audio files (WAV, AIFF, FLAC, MP3 or OGG) or playlist files (M3U, M3U8, PLS or XSPF) in the file dialog and click the **Open** button.
- Select **File \| Open Folder...** from the main menu. Then choose the folder containing audio files and click the **Open** button. 
In this case, the program will not only add audio files of the supported audio formats within the selected folder, but it
will also search audio files in all the sub-folders. The playlist files of the supported formats within the folder 
and the sub-folders will be found and parsed as well.
- Drag & Drop files/folders to the **Playlist** from anywhere possible. Just like in the previous point, the program
will also search audio files and parse the playlist files in all the dragged & dropped folders and their sub-folders.
- If the application is not opened yet, you can alternatively select audio files in File Explorer (on Windows) or Finder (on macOS) and 
use the **Open with** option in the right-click context menu to open them with EarQuiz Frequencies.

The audio items of valid (10 sec. and more) duration, which can (potentially) be opened, have normal (black) font color.
If an error occurred while trying to read a file or load it to the player, or its duration is less than 10 sec., or its sampling rate is lower than 44.1 kHz,
it would be colored with gray. If a file, having already been added to the **Playlist**, cannot be found anymore, it becomes red.

You can change the items' order with the internal drag & drop of the **Playlist**.

To show any of the tracks from the **Playlist** in File Explorer (on Windows) or Finder (on macOS), select and right-click on it (or 
select it with right-clicking) and choose the corresponding option in the context menu.

Clicking the **![]({{ site.urlimg }}Frequencies_Help/clear.png)Clear** button above the **Playlist** removes all the items from it.
To remove certain tracks, select them and click on the <span style="color:red; font-weight:bold">-</span> button, 
or choose the **Remove Selected** option from the right-click context menu, or press the *Backspace* or the *Delete* key.
There is also an option to remove the unavailable (gray and red) tracks, selecting **Remove Unavailable** from the 
right-click context menu.

#### Exporting Playlists

To export your **Playlist** contents to a separate file, select one of the two items in the **File \| Export Playlist...**
menu if the main menu. But which one to choose?

With **Export with Absolute Paths...** option, all the saved paths will be absolute. This is suitable when you are going to open the audio files
from the same machine, without changing their location or renaming drives, parent folders, etc. The playlist
file itself can be stored locally anywhere.

However, if you want to make a movable library of audio sources and organize it with playlists, you should have a separate parent folder for it, choose
**Export Using Relative Paths for Subfolders...** option, and select this folder as your playlist file location in the file dialog. In this case, the paths 
to the audio files in the same folder as the playlist file or below, would be stored as relative ones to the playlist file path. 
The other audio files' paths would be absolute.

The file dialog, which is opened on choosing any of the two options above, lets you name your playlist file, choose its future location, and
select its format/extension. Currently, you can save your playlist as M3U or M3U8 file. These are very human-readable text file formats
which may contain only audio file paths/URLs at different lines. The only difference between them is that M3U8 forces the use of UTF-8 encoding. 
On macOS, you can use them interchangeably, but on Windows the system encoding, which may be different, is used for M3U files, which may cause problems 
with non-Latin characters.
So, M3U8 is more recommended in general case.

[< Back to the Table of Contents]({{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/)