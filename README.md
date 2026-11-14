<p align="center">
  <img src="assets/icon.png" width="80" height="80" alt="EQphile Studio icon">
</p>

<h1 align="center">EQphile Studio</h1>
<p align="center"><strong>Version 0.17.8 beta</strong></p>

**A free system-wide audio equalizer for Apple Silicon Macs.**

Turn on **Mac Audio** to apply your EQ and effects to Spotify, Music, your browser and other apps.

**[Download 0.17.8 beta](https://github.com/gmaurotl/EQphileStudio/releases/tag/v0.17.8)** · [All releases](https://github.com/gmaurotl/EQphileStudio/releases) · [Installation](docs/INSTALLATION.md) · [User guide](docs/USER-GUIDE.md)

![Twenty graphic equalizer sliders and the tonal-response graph in dark mode](assets/screenshots/equalizer-en.jpg)

Each slider changes a frequency region. The **Tonal response** graph shows the combined gain from the active EQ, tone controls and preamp. For bass that overwhelms the mix, try a small cut around 105 Hz. Use the parametric mode when you want to narrow the adjustment around a specific resonance.

## Equalize your Mac in three steps

1. Start a track in Spotify or Music, or play a video in your browser.
2. Click **Mac audio** in EQphile Studio and grant system-audio access. Hover over the button and look for **Filtering** while the track plays.
3. Open **Audio → Equalizer → Bands**, turn on **Equalizer**, and choose **Use graphic EQ** if needed. Start with a small cut or boost and toggle **Equalizer** to compare.

[Full setup, including permission and output checks](docs/USER-GUIDE.md#enable-system-wide-equalization)

## Audio specifications

| Control | What you can adjust |
| --- | --- |
| **Graphic EQ** | 20 fixed bands with ±15 dB gain per band. The band centres run from 5 Hz to 20 kHz. |
| **Parametric EQ** | One peaking filter with a 20 Hz–20 kHz centre frequency, ±15 dB gain and Q from 0.2 to 12. Choose graphic or parametric mode. |
| **Tone and headroom** | Bass and treble shelves at 90 Hz and 10 kHz, each with 0 to +15 dB of boost. The preamp ranges from −30 to +15 dB. The limiter and output level meter help with peak control. |
| **Dynamic processing** | Adaptive spectral unmasking, transients, microdetail, dynamic smoothing and harmonic texture. Set intensity per effect or compare all five with the **Effects** switch. |
| **Visual feedback** | Tonal response for EQ, tone and preamp, plus a live before/after spectrum for the effects. |
| **Output format** | Select supported sample rates and bit depths for the active output. Core Audio device options can include 44.1, 48, 96 and 192 kHz, up to 384 kHz when offered by the hardware. |
| **Local audio** | FLAC, WAV, AIFF, MP3 and AAC. Mono or stereo, with a 256 MiB limit on decoded 32-bit float PCM per file. |

The EQ and effects run locally for both file playback and captured system audio. [Listening examples and DAC setup](docs/USER-GUIDE.md#tune-by-ear) · [Device and format compatibility](docs/COMPATIBILITY.md)

## Keep your music within reach

- **Local library.** Browse and play files with track information and artwork when available.
- **Apple Music, Spotify and YouTube.** See what's playing in Music for Mac, Spotify desktop or a supported browser. Artwork and playback controls depend on the source and what it makes available. Spotify and Music controls require macOS Automation permission.
- **EQphile Notch.** Bring available playback controls and artwork to the top of the screen with the optional panel.
- **Appearance.** Choose light or dark mode and an accent colour. The artwork tints the glass interface. Available in English, Spanish, French and German.

## Screenshots

### Music player

![EQphile Studio player with album artwork, a tinted background and playback controls](assets/screenshots/player-en.jpg)

The Player shows the track, album, artwork and progress. Use a local FLAC or WAV you know well, seek to the same passage and compare one adjustment at a time at a similar listening level.

### Processing

![Processing activity display and independent Transients and Microdetail controls in light mode](assets/screenshots/processing-en.jpg)

**The Clarity tab is open here.** The two dials set the intensity of Transients and Microdetail independently. The **Before** and **After** traces show what the five effects are doing to the spectrum as the signal changes. Use the **Effects** switch to compare the full effects chain while keeping your EQ and individual effect settings.

- **Clarity.** **Transients** brings out the start of a note. Listen to the snap of a snare or the attack of a plucked string. **Microdetail** lifts quieter material already present in the mix, such as the tail of a note. It can also make background noise easier to hear.
- **Smoothness.** **Unmasking** dynamically reduces dominant frequency regions. Try it when one sound makes neighbouring details harder to hear. **Dynamic smoothing** softens concentrations in the mids and highs. Listen for less bite on sharp vocals or cymbals while the rest of the track plays.
- **Texture.** **Harmonic texture** uses gentle saturation to add colour. Try a small amount on a familiar voice or bass line and compare at a similar level.

These effects work on the stereo mix. Start with one at low intensity and bring in the others as needed.

### EQphile Notch

![Expanded EQphile Notch with demo artwork, progress and playback controls](assets/screenshots/notch.png)

The expanded Notch shows the track and its progress alongside playback controls, so you can replay a passage or change tracks without leaving the EQ view. Available controls depend on the playback source.

Screenshots show demo track information and original cover artwork. The processing graph uses a test signal.

## Compatibility

The beta was tested on **macOS 27.0.1**. See [compatibility details](docs/COMPATIBILITY.md) for the technical requirements and [installation](docs/INSTALLATION.md) for the first launch and manual updates.

## Support and project

Report a bug in [Issues](https://github.com/gmaurotl/EQphileStudio/issues/new/choose) or contact [eqphile@maurotarazona.com](mailto:eqphile@maurotarazona.com) for private support. Developed by Mauro Gonzalo Tarazona-Levano. [Developer website](https://maurotarazona.com)

The app’s source code is private. If you'd like to support development, you can [leave a tip](docs/DONATIONS.md).

[Support guide](docs/SUPPORT.md) · [Privacy](docs/PRIVACY.md) · [App terms](LICENSE.txt) · [Third-party notices](docs/NOTICE.md)
