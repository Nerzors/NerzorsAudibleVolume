# Changelog


## 0.3.1 — 2026-10-22

- A separate Firefox build, starting from version 142, featuring a stable add-on ID and an explanation—with no data collection.
- The minimum required Gecko version for desktop has been lowered from 142 to 140, ensuring that Mullvad 140 does not fail due to the manifest.

## 0.2.0 — 2026-10-22

- Initial public release.
- Volume control added directly between the playback buttons and the bottom menu bar in the Audible.de web player.
- 0–100% range, settings are stored locally and restored for new audio items.
- Supports German and English (English is the default language).
- Keyboard navigation support and localized text for screen readers.
- Toggleable dark mode for the web player, with local storage and color adjustment for cover art.
- Mute button that restores the previous volume level and remembers its state.
- Supports eleven specific Audible country domains (with or without "www"); exclusively for HTTPS-based web players.
- Automated tests for domain scoping, mute functionality, player replacement, and theme states.


