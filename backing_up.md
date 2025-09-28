---
title: Backing Up
nav_order: 6
parent: Installation
---

# Backing Up MiB64

If you want to back up your MiB64 installation (e.g. before formatting your hard drive) or move it to another computer,  
you need to know where your personal settings are stored.

All support and settings files are located in a subfolder of the installation root folder:

`\\Config`

These files include:

- `AzimersMiBAudio.ini` — AziAudio-MiB configuration
- `Icepir8LLE-config.ini` — Icepir8sMiB64LLE configuration
- `NRage.ini` — NRage-MiB-Input configuration
- `MiB64.apps` — Application settings
- `MiB64.cdb` — Cheat database
- `MiB64.rdi` — Game database information
- `MiB64.rds` — Game database settings

---

Changes to [Game Settings](app-game-settings.md) are saved in `MiB64.rds`.  
This applies if you've added games or modified existing entries.

Any cheat codes you've added are saved in `MiB64.cdb`.  
Back this up if you want to keep them.

Your input configuration can be exported to a file. See your current [input plugin configuration](config-input.md).

---

Don't forget to also back up:

- Any [3rd party plugins](additional-plugins.md), if your [plugins folder](app-directories.md) is a subfolder of your MiB64 folder (default)
- Any save files, if your [Saves folder](app-directories.md) is a subfolder of your MiB64 folder (default)
- Any game files you've placed inside your MiB64 folder

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Backing Up Protocol Complete -->
