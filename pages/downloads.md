---
layout: page
title: "Downloads"
subheadline: "EarQuiz Software Releases"
permalink: "/downloads/"
---

## EarQuiz Frequencies

[GitHub Repository](https://github.com/Gdalik/EarQuiz_Frequencies) <br/>

If you cannot find the binaries, built for your platform (OS version, processor architecture), you can try to run 
(and build) the application from the source code, having installed a supported version of *Python* and all the required dependencies.
See the [README][19] file for the details.

For Windows binaries, starting from *version 0.1.5*, this program uses free code signing provided by [SignPath.io][9], 
and a certificate by the [SignPath Foundation][10].

### Version 0.1.7<br/>
*Release Date: Sep 04, 2024*

| Platform                   | Build          | Notes                                                                                                                       |
|----------------------------|----------------|-----------------------------------------------------------------------------------------------------------------------------|
| Windows (64-bit)           | [Download][15] | Tested manually on Windows 10, 11                                                                                           |
| macOS 12 or higher (Intel) | [Download][16] | For Intel processors only. <br/> Tested manually on macOS 12 (Monterey)                                                     |
| macOS (Silicon)            | [Download][17] | For Apple Silicon processors only. <br/> Tested manually on macOS 14 (Sonoma).<br/> May be incompatible with lower versions |
| Linux (amd64)              | [Download][18] | For x86-64 processors. <br/> Tested manually on Ubuntu 22.04.4                                                              |

#### What's new in version 0.1.7?

- [<img src="{{ site.urlimg }}Social/youtube_16.png"> New Features](https://youtu.be/gnop0Z-3LWg)
  - Possibility to adjust the audio processing parameters of training examples
(EQ On/Off time proportion, EQ On↔︎Off transition time, example fade in/out duration) from the dialog window, 
called by selecting **Audio | Audio Processing Settings** from the main menu, added.
  - **EQ Always On In Test Mode** option added to the **Audio** menu of the main menu.
- Old Features
  - Support of native OS audio backends deprecated.
  - Possibility to switch between *FFmpeg* and native OS audio backend deprecated.
The application now uses *FFmpeg* as the only multimedia framework on all the platforms.
- Bugs Fixed
  - The bug in Qt6/PyQt6 library that caused deadlock when using *FFmpeg* backend and led to the application hanging fixed.
  - SSL certificate added, fixing HTTPS verification issue during application updates checking process.
- GUI Changes and Improvements
  - Application style changed to 'Fusion' on Windows 11
  - Dark Mode is now supported on Windows 11, along with macOS and Linux.
  - Other minor adjustments.

### Version 0.1.6<br/>
*Release Date: Apr 25, 2024*

| Platform                   | Build           | Notes                                                                                                                       |
|----------------------------|-----------------|-----------------------------------------------------------------------------------------------------------------------------|
| Windows (64-bit)           | [Download][11]  | Tested manually on Windows 10, 11                                                                                           |
| macOS 11 or higher (Intel) | [Download][12]  | For Intel processors only. <br/> Tested manually on macOS 12 (Monterey)                                                     |
| macOS (Silicon)            | [Download][13]  | For Apple Silicon processors only. <br/> Tested manually on macOS 14 (Sonoma).<br/> May be incompatible with lower versions |
| Linux (amd64)              | [Download][14]  | For x86-64 processors. <br/> Tested manually on Ubuntu 22.04.4                                                              |

#### What's new in version 0.1.6?

- Linux is now supported!

- New Features

  - *FFmpeg* is now supported and set as the default audio backend.
  - Possibility to switch between *FFmpeg* and native system audio backend: **Audio \| Audio Playback Backend** menu added to the main menu.
  - AIFF and OGG files can be played back on all the platforms (with *FFmpeg*).

- Bugs Fixed

  - Splash Screen did not appear/disappear at the right time.
  - The application often froze on startup.
  - Mode buttons were not greyed out when disabled.
  - [on macOS] Playback position of FLAC files was often wrong when not played from start. *FFmpeg* handles it right.

- GUI Improvements

  - Font size adjustments.
  - *Arial* is now used as the main font to increase similarity across the platforms.

### Version 0.1.5<br/>
*Release Date: Mar 20, 2024*

[<img src="{{ site.urlimg }}Social/youtube_16.png"> The Dark Mode is supported on macOS now!](https://youtu.be/QNEA4jI1jw4)

| Platform                   | Build         | Notes                                                                                                                                       |
|----------------------------|---------------|---------------------------------------------------------------------------------------------------------------------------------------------|
| Windows (64-bit)           | [Download][6] | Tested manually on Windows 10, 11. <br/> Free code signing provided by [SignPath.io][9], and a certificate by the [SignPath Foundation][10] |
| macOS 11 or higher (Intel) | [Download][7] | For Intel processors only. <br/> Tested manually on macOS 12                                                                                |
| macOS (Silicon)            | [Download][8] | For Apple Silicon processors only. <br/> Tested manually on macOS 13, 14.<br/> May be incompatible with lower versions                      |

### Version 0.1.4<br/>
*Release Date: Feb 20, 2024*

***Apple Silicon processors are now supported!***


| Platform           | Build         | Notes                                                                                                                   |
|--------------------|---------------|-------------------------------------------------------------------------------------------------------------------------|
| Windows (64-bit)   | [Download][3] | Tested on Windows 10, 11                                                                                                |
| macOS 11 or higher | [Download][4] | For Intel processors only <br/> Tested on macOS 12                                                                      |
| macOS (Silicon)    | [Download][5] | For Apple Silicon processors only. <br/> Tested manually on macOS 13, 14.<br/> May be incompatible with lower versions  |


### Version 0.1.3 <br/>
*Release Date: Feb 01, 2024*

[Source Code (zip)](https://github.com/Gdalik/EarQuiz_Frequencies/archive/refs/tags/EarQuiz_Frequencies-v0.1.3.zip) <br/>
[Source Code (tar.gz)](https://github.com/Gdalik/EarQuiz_Frequencies/archive/refs/tags/EarQuiz_Frequencies-v0.1.3.tar.gz) <br/>
*Tested with Python 3.9, 3.10*

| Platform | Build         | Notes                       |
|----------|---------------|-----------------------------|
|Windows (64-bit) | [Download][1] | Tested on Windows 10, 11    |
| macOS 11 or higher | [Download][2] | For Intel processors only   |

[1]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.3/eqfreq_v0.1.3.build-9.exe
[2]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.3/EarQuiz.Frequencies.v0.1.3.pkg
[3]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.4/eqfreq_v0.1.4-Windows.exe
[4]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.4/EarQuiz_Frequencies-v0.1.4-macOS-Intel.pkg
[5]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.4/EarQuiz_Frequencies-v0.1.4-macOS-Silicon.dmg
[6]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.5/eqfreq_v0.1.5-Windows.exe
[7]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.5/EarQuiz_Frequencies_v0.1.5-macOS-Intel.pkg
[8]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.5/EarQuiz_Frequencies_v0.1.5-macOS-Silicon.dmg
[9]: https://signpath.io/
[10]: https://signpath.org/
[11]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.6/eqfreq_v0.1.6-build-39-Windows.exe
[12]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.6/EarQuiz_Frequencies_v0.1.6-macOS-Intel.pkg
[13]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.6/EarQuiz_Frequencies_v0.1.6-macOS-Silicon.dmg
[14]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.6/earquiz-frequencies_0.1.6-01_amd64.deb
[15]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.7/eqfreq_v0.1.7-build-42.exe
[16]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.7/EarQuiz_Frequencies-v0.1.7-macOS-Intel.pkg
[17]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.7/EarQuiz_Frequencies-v0.1.7-macOS-Silicon.dmg
[18]: https://github.com/Gdalik/EarQuiz_Frequencies/releases/download/EarQuiz_Frequencies-v0.1.7/earquiz-frequencies_0.1.7-01_amd64.deb
[19]: https://github.com/Gdalik/EarQuiz_Frequencies/blob/master/README.md