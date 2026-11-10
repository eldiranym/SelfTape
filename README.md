# ColdRead

Offline script rehearsal for Apple Silicon Macs, with Kokoro scene-partner voices.

This repository hosts downloadable releases and the corresponding source for the bundled speech helper. The public edition includes Kokoro only.

## Release status

The first release is being prepared. There is no published installer yet. Developer ID signing, Apple notarization, and testing on a separate Mac remain pending.

## Planned requirements

- Apple Silicon Mac (M-series)
- macOS 15 or later; the oldest supported release still needs device testing
- Microphone and Speech Recognition permission for spoken rehearsals

The voice model and all 54 voices are bundled. Rehearsals run on the Mac without a cloud speech service or a voice download. Apple on-device speech recognition availability is checked before rehearsal.

## Licenses and source

Each binary release will include third-party notices and a matching `ColdRead-Kokoro-Corresponding-Source.zip` asset. That source archive covers the bundled speech helper and its dependencies; it is not required to run the app. Component licenses are also accessible from the app's Third-Party Licenses menu.
