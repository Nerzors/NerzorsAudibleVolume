<div align="center">
<img src="https://media.nerzors.de/img/_projects/NAV_NerzorsAudibleVolume.png" alt="Nerzors Audible Volume Logo Images"/>

<h1>Nerzors Audible Volume</h1>

<p><i>If they don’t do it, then I do it myself!</i></p>

<p>
  <img src="https://img.shields.io/badge/Chrome_Web_Store-Coming_soon-1B1F2B?style=for-the-badge&logo=googlechrome&logoColor=4285F4&labelColor=1B1F2B" alt="Chrome Web Store - coming soon"/>
  <!-- <a href="#">
    <img src="https://img.shields.io/badge/Firefox_Add--ons-Install-1B1F2B?style=for-the-badge&logo=firefoxbrowser&logoColor=FF7139&labelColor=1B1F2B" alt="Firefox Add-ons"/>
  </a> -->
</p>

<!-- Tested on :> -->
<p>
  <img src="https://img.shields.io/badge/Tested%20on-Google%20Chrome-1B1F2B?style=for-the-badge&logo=googlechrome&logoColor=4285F4&labelColor=1B1F2B" alt="Tested on Google Chrome"/>
  <img src="https://img.shields.io/badge/Tested%20on-Firefox-1B1F2B?style=for-the-badge&logo=firefoxbrowser&logoColor=FF7139&labelColor=1B1F2B" alt="Tested on Firefox"/>
  <img src="https://img.shields.io/badge/Tested%20on-Mullvad%20Browser-1B1F2B?style=for-the-badge&labelColor=1B1F2B" alt="Tested on Mullvad Browser"/>
  <img src="https://img.shields.io/badge/Tested%20on-Opera-1B1F2B?style=for-the-badge&logo=opera&logoColor=FF1B2D&labelColor=1B1F2B" alt="Tested on Opera"/>
  <img src="https://img.shields.io/badge/Tested%20on-Opera%20GX-1B1F2B?style=for-the-badge&logo=operagx&logoColor=FA1E4E&labelColor=1B1F2B" alt="Tested on Opera GX"/>
</p>

<p>
  <img src="https://img.shields.io/github/v/release/Nerzors/NerzorsAudibleVolume?style=flat-square&color=252669&labelColor=1B1F2B" alt="Latest Release"/>
  <img src="https://img.shields.io/github/last-commit/Nerzors/NerzorsAudibleVolume?style=flat-square&color=A87CE8&labelColor=1B1F2B" alt="Last Commit"/>
  <img src="https://img.shields.io/github/issues/Nerzors/NerzorsAudibleVolume?style=flat-square&color=252669&labelColor=1B1F2B" alt="Open Issues"/>
  <img src="https://img.shields.io/github/stars/Nerzors/NerzorsAudibleVolume?style=flat-square&color=A87CE8&labelColor=1B1F2B" alt="Stars"/>
</p>


[Install](#installation) &nbsp;|&nbsp; [Features](#features) &nbsp;|&nbsp; [Issues](#if-the-controller-is-missing) &nbsp;|&nbsp; [Privacy](#privacy-and-license) &nbsp;|&nbsp; [Changelog](CHANGELOG.md)

</div>

> [!IMPORTANT]
> Independent project, **not affiliated with Audible or Amazon**. Manual installation is currently available, a store listing is planned.

## Features

- Volume control from 0 to 100%, directly below the playback buttons in the Audible web player.
- Settings are saved locally and applied when the player is reopened.
- Supports keyboard control, displays volume as a percentage, and automatically adjusts for dynamically loaded audio elements.
- Language (German or English) is determined by the browser's language setting, English serves as the default and fallback.
- No tracking or data transmission by the extension.
- Speaker icon for muting and unmuting.
- Toggle for dark mode (moon/sun icon); preferences are saved locally. Default is light mode.

## Installation

### Chromium
Manual installation - Chrome, Opera and Opera GX. No Node.js installation is required for the ready-to-use ZIP.

1. Download the latest release ZIP, for example `NerzorsAudibleVolume-v0.3.1-chromium.zip` from [Releases](https://github.com/Nerzors/NerzorsAudibleVolume/releases).
2. Extract the entire contents of the ZIP file into a permanent folder. Do not move or delete this folder afterward, as the browser loads the extension from that location.
3. In Chrome, open `chrome://extensions`. In Opera and Opera GX, open `opera://extensions`.
4. Enable **Developer mode**.
5. Click **Load unpacked** and select the folder you extracted-the one that contains the `manifest.json` file directly.
6. Open `https://www.audible.de/webplayer` or reload the player if it is already open.

The control appears between the playback buttons and the speed/chapters/bookmarks section. There is no need to click an extension icon. The extension uses its own logo.

If you have downloaded the entire version folder, you can alternatively load its `extension` subfolder directly. The ZIP file is the ready-to-use extension itself, not a source code archive.

### Firefox & Mullvad

The Firefox package requires **Firefox and Mullvad 140 or newer**.

1. Download `NerzorsAudibleVolume-v0.3.1-firefox.zip` from the matching release and extract it.
2. Open `about:debugging#/runtime/this-firefox` in Firefox or Mullvad.
3. Select **Load Temporary Add-on** and choose the extracted `manifest.json`.
4. Open or reload an allowed Audible web player and now use volume, mute & dark mode.
5. If the controls do not appear, check the extension's website access in the add-on settings.

> Temporary add-ons are removed when Firefox restarts. A ZIP is **not** a permanently installable signed Firefox add-on. Normal distribution requires Mozilla signing; no signing or AMO submission is performed by this project script. See [Mozilla's temporary installation guide](https://extensionworkshop.com/documentation/develop/temporary-installation-in-firefox/).

## Update and Remove

Updates do not occur automatically with a manual installation. Unpack the new ZIP version into the same extension folder and replace the existing files.
Also, remove any files that are no longer included in the new version. Afterward, select **Reload** in the extension manager and refresh the Audible page.
Do not uninstall the extension before updating, as this ensures your local settings are preserved.

To remove the extension, select **Remove** in the extension manager and refresh the player page.

### If the controller is missing

- Check that the extension is enabled and the correct folder is loaded.
- Reload the web player on an authorized Audible domain (see below).
- Check for error messages in the extension management settings.
- The controller is disabled by default if no audio element is present. Audible may change its DOM structure, which could necessitate an update.

Or create a bug report under [Issues](https://github.com/Nerzors/NerzorsAudibleVolume/issues)

## Privacy and License

Volume, the last audible value, mute status, and dark mode selection are stored locally via `chrome.storage.local`.
Permissions: `storage` and content script access to the Audible web player. Further details can be found in [PRIVACY.md](PRIVACY.md).
The source code is licensed under the [MIT License](LICENSE). **Audible and Amazon are trademarks of their respective owners.**

## Allowed domains

`audible.de`, `audible.com`, `audible.co.uk`, `audible.ca`, `audible.com.au`, `audible.fr`, `audible.co.jp`, `audible.it`, `audible.in`, `audible.es`, `audible.com.br`. Each with and without `www`, only HTTPS and `/webplayer`. Source: [Audible Marketplaces](https://help.audible.com/s/article/update-your-country-marketplace?language=en_US).

Allowing a domain does not establish that its regional player has been tested separately. Dark Mode uses color filtering with compensation for covers and the extension controls, different player versions, graphics or overlays may require further adjustments. If necessary, confirm new page permissions in the browser when updating.

## Tested browsers

Version 0.2.0 was successfully tested in:

- Google Chrome (155)
- Opera
- Opera GX (137)

whit Version 0.3.1:

- Firefox
- Mullvad Browser (140)
