# EQphile Studio user guide

[Enable system-wide equalization](#enable-system-wide-equalization) · [Choose an EQ mode](#choose-an-eq-mode) · [Tune by ear](#tune-by-ear) · [Set up a USB DAC](#set-up-a-usb-dac) · [Troubleshooting](#troubleshooting)

## Enable system-wide equalization

1. Select your headphones, speakers or USB DAC in **System Settings → Sound → Output**. Start a track in Spotify or Music, or play a video in your browser.
2. Open EQphile Studio and click **Mac audio**, the speaker button in the transport bar or beneath the progress bar in **Player**.
3. On first use, allow access to system audio when macOS asks. You can review the permission in **System Settings → Privacy & Security → Screen & System Audio Recording**. If macOS lists **System Audio Recording Only** separately, use the audio-only entry there. Follow any relaunch prompt and click **Mac audio** again if needed. [Apple’s guide to system audio permissions](https://support.apple.com/guide/mac-help/control-access-screen-system-audio-recording-mchld6aa7d23/mac)
4. Hover over **Mac audio** while the other app is playing. **Filtering · [device] · [rate] Hz** confirms that Studio is receiving and filtering audio on the named output. **Listening** means no signal is currently detected. If you see **Waiting for audio or permission**, the original output remains active.
5. Go to **Audio → Equalizer → Bands**. With **Equalizer** on and **Active mode** shown, temporarily lower the **940 Hz** slider by a few dB on a track with vocals. Toggle **Equalizer** to hear the change, then return the band to its starting value. This compares the selected EQ mode while leaving Tone and Processing in their current states.

Click **Mac audio** again to stop system-wide processing. EQphile Studio applies the same sound controls to files played in its own Player. Spotify, Music and browser source selectors are for track information and available playback controls. You can equalize their audio without selecting them as the Player source.

## Choose an EQ mode

- **Bands** gives you 20 sliders for shaping several parts of the spectrum. Choose **Use graphic EQ** if Parametric is active.
- **Parametric** gives you one bell filter for a particular frequency. Set its **Frequency**, **Gain** and **Q**. A higher Q makes the adjustment narrower. Choose **Use parametric EQ** to make it active.
- **Tone** adds independent bass and treble boosts that work with either EQ mode. **Preamplifier** trims the overall EQ gain to leave headroom for boosts. **Limiter** helps control peaks.

Only one EQ mode runs at a time. **Tonal response** shows the combined curve of the active EQ, tone and preamp. For a repeatable setup, open **Presets** to save your EQ, tone and preamp values. Presets can be exported and imported as JSON. Right-click a slider or dial to enter a numerical value.

## Tune by ear

Start with a recording you know and change one control at a time. Compare at a similar listening volume so that loudness does not decide the comparison.

| What you want to hear | What to try |
| --- | --- |
| Less bass bloom | In **Bands**, start with a small cut at **105 Hz**. Try **165 Hz** if the excess is higher. |
| Less bite from vocals or cymbals | Try a small cut at **3.5 kHz** in **Bands**. For a narrow resonance you can locate, use **Parametric** with a negative gain and adjust Q. If harshness varies from moment to moment, try **Dynamic smoothing** at low intensity. |
| More definition from drums or plucked strings | In **Processing → Clarity**, raise **Transients** gradually. Try **Microdetail** separately to lift quiet elements. It can also make background noise more noticeable. |
| More room around a dominant sound | In **Processing → Smoothness**, try **Unmasking** at low intensity. It reduces prominent frequency regions dynamically within the stereo mix. |
| A warmer tone | In **Processing → Texture**, try a small amount of **Harmonic texture** for gentle saturation. |

Under **Audio → Processing**, each effect has a switch and an intensity dial. Use **Effects** to compare all five together with your selections preserved. **Processing activity** shows the spectrum before and after those effects while audio is playing. Use **Audio → Output** to monitor the output level. If you see **Clipping · lower Preamp**, reduce **Preamplifier** in **Audio → Equalizer → Tone**. Several boosts can overlap, so judge headroom on the loudest passage you plan to play.

## Set up a USB DAC

1. Connect the DAC by USB and select it in **System Settings → Sound → Output**.
2. In Studio, go to **Audio → Output**. Confirm the device name and active format.
3. Choose an available sample rate and bit depth, then click **Apply**. For a loaded local file, **Match audio file** is available when the device supports the file’s sample rate. A format change can briefly interrupt playback.

The options come from the device and its connection. Bluetooth rate and bit-depth controls are read-only in Studio. The displayed sample rate and bit depth describe the output format. Setting them higher does not restore source detail, and active EQ or effects change the audio samples.

## Troubleshooting

- **Listening or waiting.** Keep a track playing in another app, confirm that it uses the default Mac output, and check Studio’s audio permission. Try toggling **Mac audio** off and back on.
- **The sound is unchanged.** Check **Filtering**, the **Equalizer** switch and **Active mode**. Use **Tone** for the shelves and **Effects** plus each individual switch for the five processors.
- **No sound after changing outputs.** Turn off **Mac audio**, check that ordinary playback returns on the selected output, then turn it back on. If the issue repeats, include your macOS version, source app and output device in a [support report](SUPPORT.md).
