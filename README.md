# SelfTape

Offline script rehearsal for Apple Silicon Macs. Import your sides, choose your role,
and let Kokoro read the other characters while the app follows your spoken lines.

## Download

[SelfTape 1.2.6 preview release](https://github.com/eldiranym/SelfTape/releases/tag/v1.2.6)

| Edition | Download | Installed size | Included model |
| --- | --- | --- | --- |
| [SelfTape](https://github.com/eldiranym/SelfTape/releases/download/v1.2.6/SelfTape-1.2.6-arm64-preview.dmg) | 344 MB | 407 MB | Full-precision Kokoro |
| [SelfTape Lite](https://github.com/eldiranym/SelfTape/releases/download/v1.2.6/SelfTape-Lite-1.2.6-arm64-preview.dmg) | 131 MB | 196 MB | 8-bit Kokoro |

Both include 28 English voices (20 American and 8 British) and the native in-process
Kokoro speech engine with a 512 MiB persistent disk cache. Lite reduces download size
by about 62%; it is not a speed upgrade and quantization can change voice quality.
Choose SelfTape unless the smaller download and disk footprint are your priority.

Each edition has its own app identity, script library, and speech cache, and can be
installed alongside the other. Rehearsal audio and scripts are processed on your Mac,
with no cloud speech service, account, Python installation, helper process, or
voice-model download. On-device speech recognition availability is checked before rehearsal.

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

- PDF import, including scanned pages with on-device OCR and watermark filtering
- Word DOCX, Final Draft, Fountain and plain-text scripts
- Character casting from 28 bundled English Kokoro voices with native in-process synthesis
- Persistent 512 MiB speech cache for instant repeat rehearsals
- Self Tape and Memorize rehearsal modes
- Offline speech recognition, transcript display, adjustable reader pace and pauses
- Studio interface with light/dark appearance and importable themes

## Licenses and checksums

Third-party notices are bundled inside the app and accessible from the app's
Third-Party Licenses menu. `SHA256SUMS.txt` on the release page covers both DMG
installers.

## Easy updates

Versions 1.2.1 and newer include automatic daily update checks and **Check for Updates…** in the
app menu. When an update is available, choose Install Update, then Install and
Relaunch. You can switch automatic checks off in the same menu. Update downloads
and feeds are signed, and each edition stays on its own update feed.

**If you installed 1.2.0, download and install 1.2.6 manually once.** Future updates
can then happen inside the app. Update checks need internet; rehearsal speech
remains on your Mac. These previews still require initial macOS approval.
