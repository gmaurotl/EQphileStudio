# Installation and manual updates

EQphile Studio **0.17.8 (40)** — Apple Silicon beta.

## Download and verify

Download both files from the [official 0.17.8 beta release](https://github.com/gmaurotl/EQphileStudio/releases/tag/v0.17.8):

- **EQphileStudio-0.17.8-arm64.zip** — the compiled Mac app.
- **SHA256SUMS.txt** — the checksum for that ZIP.

GitHub's automatically generated **Source code** archives contain this
repository's documentation, not the installable app or its private source.

To verify the ZIP, open Terminal in the folder containing both downloaded files
and run this optional integrity check:

```sh
shasum -a 256 -c SHA256SUMS.txt
```

The result should be `EQphileStudio-0.17.8-arm64.zip: OK`. Stop if it does not
match and download the files again from the same release. A checksum verifies
file integrity; it does not replace developer signing or notarization.

## Install the app

1. Open the ZIP in Finder.
2. Drag **EQphile Studio.app** into **Applications**. The ZIP contains the app;
   there is no installer, activation key or payment step.
3. Open EQphile Studio from Applications.

This beta is **ad hoc signed, without Developer ID or Apple notarization**.
macOS may block its first launch. Apple's [opening guidance](https://support.apple.com/en-us/102445)
describes the per-app exception in System Settings → Privacy & Security for
software you choose to trust. Do not disable Gatekeeper globally. If macOS says
the app will damage your computer, stop and report the exact alert to support.
First launch on another Mac or in a fresh user account has not been verified.

## First use

- **Local files:** add an audio file in the library or player.
- **Spotify:** open the desktop Spotify app, play a track and select Spotify in Studio.
- **Music / Apple Music:** play a track in Music, then select that source in Studio.
- **Browser / YouTube:** play media in a supported browser and select the browser source.
- **Mac Audio:** enable it separately to process other apps' sound. Grant the
  system-audio permission when macOS asks for this feature.

Spotify and Music controls require their respective macOS Automation permissions.
Streaming-service access remains with those apps; Studio does not provide a
service subscription. See [Compatibility](COMPATIBILITY.md) for limits, including
artwork availability and the macOS versions actually tested.

## Update manually

Public update checks are disabled in this build; it does not download or install
updates automatically. To use a later version:

1. Download that release's ZIP and its matching checksum file.
2. Verify the download, then quit Studio with **⌘Q** before replacing it.
3. Replace the installed app in Applications and open the new version.

Replacing the app does not require deleting your original music, preferences or
presets. Read each release's notes for any version-specific migration steps.

## Support and terms

All included features are free and the application source stays private.
Read the [binary terms](LICENSE.txt), [privacy information](PRIVACY.md) and
[third-party notices](NOTICE.md), also available offline in the app's Help menu.

Support: **eqphile@maurotarazona.com**.

Developer website: [maurotarazona.com](https://maurotarazona.com).
