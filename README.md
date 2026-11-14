<img src="assets/icon.png" width="80" height="80" alt="EQphile Studio icon">

# EQphile Studio

**A free system-wide audio equalizer for Apple Silicon Macs.**

Turn on **Mac Audio** to apply your EQ and effects to Spotify, Music, your browser and other apps.

**[Download 0.17.8 beta](https://github.com/gmaurotl/EQphileStudio/releases/tag/v0.17.8)** · [Installation](docs/INSTALLATION.md) · [User guide](docs/USER-GUIDE.md)

![Twenty graphic equalizer sliders and the tonal-response graph in dark mode](assets/screenshots/equalizer-en.jpg)

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

### Processing

![Processing activity display and independent Transients and Microdetail controls in light mode](assets/screenshots/processing-en.jpg)

### EQphile Notch

![Expanded EQphile Notch with demo artwork, progress and playback controls](assets/screenshots/notch.png)

Screenshots show demo track information and original cover artwork. The processing graph uses a test signal.

## Compatibility

The beta was tested on **macOS 27.0.1**. See [compatibility details](docs/COMPATIBILITY.md) for the technical requirements and [installation](docs/INSTALLATION.md) for the first launch and manual updates.

## Support and project

Report a bug in [Issues](https://github.com/gmaurotl/EQphileStudio/issues/new/choose) or contact [eqphile@maurotarazona.com](mailto:eqphile@maurotarazona.com) for private support. Developed by Mauro Gonzalo Tarazona-Levano. [Developer website](https://maurotarazona.com)

The app’s source code is private. If you'd like to support development, you can [leave a tip](docs/DONATIONS.md).

[Support guide](docs/SUPPORT.md) · [Privacy](docs/PRIVACY.md) · [App terms](LICENSE.txt) · [Third-party notices](docs/NOTICE.md)
