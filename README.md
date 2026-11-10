# SelfTape

Offline script rehearsal for Apple Silicon Macs. Import your sides, choose your role,
and let Kokoro read the other characters while the app follows your spoken lines.

## Download

[SelfTape 1.2.1 preview release](https://github.com/eldiranym/SelfTape/releases/tag/v1.2.1)

| Edition | Download | Installed size | Included model |
| --- | --- | --- | --- |
| [SelfTape](https://github.com/eldiranym/SelfTape/releases/download/v1.2.1/SelfTape-1.2.1-arm64-preview.dmg) | 416 MB | 525 MB | Full-precision Kokoro |
| [SelfTape Lite](https://github.com/eldiranym/SelfTape/releases/download/v1.2.1/SelfTape-Lite-1.2.1-arm64-preview.dmg) | 203 MB | 314 MB | 8-bit Kokoro |

Both include all 54 voices and the offline speech runtime. Lite reduces download
size by about 51%; it is not a speed upgrade. In our validation on one Mac, Lite
took about five times as long to generate speech, while still generating faster
than playback. Quantization can also change the sound. Choose SelfTape unless
the smaller download and disk footprint are your priority.

Each edition has its own app identity and script library and can be installed
alongside the other. Rehearsal audio and scripts are processed on your Mac, with
no cloud speech service, account, Python installation or voice-model download.
On-device speech recognition availability is checked before rehearsal.

## Install this preview

Requires Apple Silicon (M-series) and targets macOS 15 or newer. Device testing
was performed on macOS 27.2; earlier supported versions still need device testing.

1. Download either DMG, open it, and drag the app into Applications.
2. Open the app. These previews use a local signing certificate and **are not
   Apple-notarized or Developer ID-signed**. macOS may block the first launch.
   Review [Apple's guidance for opening apps](https://support.apple.com/en-us/102445).
   If you choose to allow this app, the per-app control is in System Settings →
   Privacy & Security → Open Anyway after the blocked launch.
3. Import a script or try the sample. Preparing a rehearsal requests microphone
   and Speech Recognition permissions for that edition.

## Features

- PDF import, including scanned pages with on-device OCR
- Word DOCX, Final Draft, Fountain and plain-text scripts
- Character casting from 54 bundled Kokoro voices
- Self Tape and Memorize rehearsal modes
- Offline speech recognition and adjustable reader pace

## Licenses and source

Third-party notices are accessible from the app's Third-Party Licenses menu.
The release also includes `SelfTape-Kokoro-Corresponding-Source.zip`, the matching
source for the bundled speech helper and its dependencies. **You do not need
that source archive to run the app.** `SHA256SUMS.txt` covers both installers and
the source archive. Component licenses are included with their source materials.

## Easy updates

Version 1.2.1 adds automatic daily update checks and **Check for Updates…** in the
app menu. When an update is available, choose Install Update, then Install and
Relaunch. You can switch automatic checks off in the same menu. Update downloads
and feeds are signed, and each edition stays on its own update feed.

**If you installed 1.2.0, download and install 1.2.1 manually once.** Future updates
can then happen inside the app. Update checks need internet; rehearsal speech
remains on your Mac. These previews still require initial macOS approval.
