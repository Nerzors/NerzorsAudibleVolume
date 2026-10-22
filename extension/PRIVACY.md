# Datenschutz / Privacy

Stand / Updated: 2026-10-22 · Version 0.2.0

## Deutsch

Nerzors Audible Volume speichert die gewählte Lautstärke, den letzten hörbaren Wert, Stummschaltung und Dark-Mode-Auswahl lokal im Browserprofil über `chrome.storage.local`. Es gibt kein Tracking, keine Analysewerkzeuge und keine von der Erweiterung veranlasste Übertragung an externe Dienste.

Das Content Script greift in den freigegebenen Audible-Webplayern auf die Playersteuerung und Audioelemente zu, um den Regler einzufügen und die Lautstärke anzupassen. Es liest keine Kontodaten, Cookies, Hörbuchinhalte oder den Browserverlauf aus.

Die Berechtigung `storage` dient dem Speichern der Einstellung. Der Seitenzugriff beschränkt sich auf HTTPS-Webplayer der elf Länder-Domains `audible.de`, `audible.com`, `audible.co.uk`, `audible.ca`, `audible.com.au`, `audible.fr`, `audible.co.jp`, `audible.it`, `audible.in`, `audible.es` und `audible.com.br`, mit und ohne `www`. Im Code werden Domain und der Pfad `/webplayer` zusätzlich geprüft. Beim Entfernen der Erweiterung werden ihre lokalen Einstellungen entfernt. Audibles eigener Datenverarbeitung liegt dessen Datenschutzerklärung zugrunde.

## English

Nerzors Audible Volume stores the selected volume, previous audible volume, mute state and dark-mode selection locally in the browser profile using `chrome.storage.local`. It contains no tracking or analytics and initiates no transmission to external services.

The content script accesses player controls and audio elements in the allowed Audible web players to insert the slider and adjust volume. It does not read account details, cookies, audiobook content, or browsing history.

The `storage` permission is used to save the setting. Page access is limited to HTTPS `/webplayer` pages on the eleven marketplace domains listed above, with or without `www`. The code additionally checks the exact hostname and path. Removing the extension removes its local settings. Audible's own data processing is governed by its privacy policy.
