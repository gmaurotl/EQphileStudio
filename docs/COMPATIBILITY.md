# Compatibility and beta scope

**EQphile Studio 0.17.8 beta (40)**.
EQphile Studio is for Apple Silicon Macs. This build does not support Intel.
The executable deployment target is macOS 14.2; that is a technical build target,
not evidence that every later release has been tested.

| Environment | Status |
| --- | --- |
| macOS 27.0.1, Apple Silicon, developer Mac | Native UI and source integrations have been exercised on this Mac. Version 0.17.8 passed release checks and simulated Spotify and browser playback tests. First-download installation on another Mac was not tested. |
| Other macOS versions from 14.2 onward | Unverified; compatibility is not promised. |
| macOS earlier than 14.2 | Not supported. |
| Intel Macs | Not supported. |

## Sources and permissions

- **Local files:** mono/stereo; up to 256 MiB of decoded float32 PCM.
- **Spotify:** desktop app and macOS Automation permission. Artwork uses approved
  Spotify image hosts; available controls depend on the source and service.
- **Music / Apple Music:** the local Music app and macOS Automation permission.
  Supports metadata, available artwork, play/pause, previous/next, seeking,
  shuffle and repeat off/all/one. Music supplies subscription content under its
  own terms. Artwork comes only from Music or matching local macOS information;
  some tracks may have no available cover.
- **Browser / YouTube:** availability depends on macOS Now Playing, the browser,
  the source and the commands it publishes. No extension is required. The
  integration uses a bundled adapter to private system media APIs, so OS changes
  can affect it.
- **Mac Audio:** system-audio permission; processing must be enabled separately
  from source selection. Supported output formats depend on the audio device.

## Validation scope

First launch on another Mac or in a fresh user account has not been verified.
Other macOS versions and audio hardware have not been verified with this beta.

For reports, include app/macOS versions, Mac chip, source, output device and
reproduction steps. Send private details to **eqphile@maurotarazona.com**;
see [Support](SUPPORT.md).

## Spotify control availability

Version 0.17.8 checks the current source, process, track and available actions.
It does not identify or certify a Premium subscription. Missing, stale or
restricted capabilities keep the affected controls disabled. Native capability
checks depend on macOS and Spotify publishing matching playback information.
The player still displays track information and progress. Open Spotify for
controls that cannot be verified. Tests use simulated contexts; no new live
Spotify account, audio output or listening test was performed.
