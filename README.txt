This is a fork of sndcpy that uses ffmpeg on GNU/Linux to reproduce the audio.
To read the original README please refer to README_sndcpy.md

Why? Well, VLC keeps on adding delay, which is really annoying. While ffmpeg's delay is still very
noticiable, it doesn't change.

You will need a PulseAudio server for this to work, the PipeWire wrapper works just fine.

On Windows this still uses VLC. No idea what's up with macOS.

If the audio pitch or speed sounds wrong, try changing the asetrate parameter
in the ffmpeg arguments. See https://github.com/audiojs/sample-rate#sample-rate---
for a table of common sample rates.

