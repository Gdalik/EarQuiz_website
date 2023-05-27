#### Pink Noise

Pink noise is a kind of random noise which has equal energy in different octave ranges. It derives from white noise which
is a random signal with wide frequency range and equal power for each frequency. Since the number of frequencies in octave doubles
for each octave increase, the energy of white noise doubles in each higher octave as well, which is 3 dB/oct. boost. In other words, white noise
gives the *impression* of high-frequencies dominance.
In pink noise, the energy falls proportionally to frequency. I.e., it is similar to white noise, but with 3 dB/octave attenuation, starting from 1 Hz. 
This gives a much more even result from a human ear perspective, and the spectrum of pink noise is the closest one to an average music signal.

[< Back to "The Basic Training Method"](basic-training-method/)

#### Peak Normalization

Peak normalization of an audio file or its part is a linear change of its whole gain that makes the amplitude level of its (PCM) sample 
with the maximum amplitude equal to a certain value (in dB).

[< Back to "Checking Audio Playback"](checking-audio-playback/)<br />
[< Back to "Setting Volume Level"](adjusting-audio-system/#setting-volume-level)

#### Supported Audio Formats
The fully supported audio formats are: WAVE, AIFF, MP3 and FLAC. The OGG format is half-supported.
OGG audio files can be added to the **Playlist**, but they cannot be played with the current media
player backend neither on Windows nor on macOS. If you try to load an OGG file, you will get the error message
with option to proceed with conversion to WAVE or AIFF. There is also a known backend issue with incorrect FLAC files'
playback position on macOS, which may occur when starting playing from a non-zero position. To work around
these format problems, you can convert audio files to WAVE or AIFF beforehand by selecting them and choosing 
**File | Convert Selected Files...** from the main menu or the similar option from the right-click context menu of the **Playlist**.

[< Back to "The Basic Training Method"](basic-training-method/)<br />
[< Back to "Working with External Audio Files"](working-with-external-audio-files/)