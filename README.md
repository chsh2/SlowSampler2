# Slow Sampler 2: A Plug-in for Audio Stretching & Tuning

Slow Sampler 2 is a 

The plug-in is originally developed for creating OtoMAD (音MAD) and YTPMV audio. Nevertheless, the application is not limited to these genres.

## Features
- Generate 16-voice polyphony sound by sampling either an audio file or an audio track in real time
- Tune the sample with several algorithms to choose from
    - Convert off-key samples to constant pitch
    - Adjust pitch & formant separately
- Time-stretch an audio sample in various ways
    - Change the playback speed, supporting a non-linear speed curve
    - A unique mode that fits the audio to the MIDI note length
- Per-voice built-in effects
    - Noise reduction & comb filters for audio enhancement
    - Modulators & vocoders using another audio sample for creative sound design

## Installation

https://steinbergmedia.github.io/vst3_dev_portal/pages/Technical+Documentation/Locations+Format/Plugin+Locations.html

## Usage

### Using Slow Sampler as a VST3 plug-in


### Using Slow Sampler as a Pure Data patch

[PlugData](https://plugdata.org/) is an environment for running/editing Pure Data programs. It can be used either as a standalone app, an instrument plugin or an effect plugin. By loading the file `plugdata.pd`, you can run Slow Sampler 2 inside PlugData in any of these modes. This way also allows the user to make some changes to the functionality of this plug-in without recompiling it.

It is less recommended to run Slow Sampler 2 with the vanilla [Pure Data](https://puredata.info/), because the patch is not compatible with the latest Pure Data release. Moreover, it contains several external objects which need to be manually installed in Pure Data. If you insist on doing this, please refer to https://github.com/chsh2/Camomile for the required dependencies.

## Compilation

To compile the project to VST3 and probably other formats of audio plug-ins by yourself, please:

- Build [this fork of Camomile](https://github.com/chsh2/Camomile) following its instructions.
- Copy all files from the release of this repository, and replace the library files with your build.
  - Please refer to Camomile's [Wiki page](https://github.com/pierreguillot/Camomile/wiki/How-to-create-new-plugins) for different configuration options.

## Credits

- Codes
    - [Pure Data](https://puredata.info/) by Miller Puckette and others
    - [libpd](https://github.com/libpd/libpd) by the Peter Brinkmann, Dan Wilcox and others
    - [PlugData](https://plugdata.org/) by Timothy Schoen and others
    - [Camomile](https://github.com/pierreguillot/Camomile) by Pierre Guillot and others
    - [ELSE](https://github.com/porres/pd-else) by Alexandre Torres Porres
    - [Cyclone](https://github.com/porres/pd-cyclone) by Krzysztof Czaja, Hans-Christoph Steiner, Fred Jan Kraan, Alexandre Porres, Derek Kwan, Matt Barber and others
- Resources
    - Some icon images from [Iconbuddy](https://iconbuddy.app/)
    - Font: [Sarasa Gothic](https://github.com/be5invis/Sarasa-Gothic)
    - Font: Calistoga