---
title: Keeping Current
nav_order: 4
parent: Installation
---

# Updating MiB64 Files

The first thing, of course, is to check you have the **latest version of MiB64** by visiting the official site—see [Web Links](web_links.md).

Check if any of the plugins have been updated. This could make a large difference to your results.  
Keep an eye on any third-party plugins included with MiB64 that you are using, as they may be updated independently of MiB64.

Aside from executable code (`.exe` and `.dll` files), MiB64 uses several plain text files which are likely to be updated more frequently:

---

### `MiB64.rds` — Game Database Settings

Updates to this file could help you get more games working by:

- Providing correct settings for each game
- Correcting mistakes in existing entries
- Improving user instructions in the Notes fields
- Correcting status designations

This is an important file to keep updated. See [Web Links](web_links.md).

---

### `MiB64.cdb` — Cheat Code Database

Updates to this file may:

- Add more cheat codes
- Correct existing cheat codes
- Remove problematic or non-working cheats
- Improve guidance notes

See [Web Links](web_links.md).

---

### `MiB64.rdi` — Game Database Information

Updates to this file can provide extra information for games in the Game Browser, such as Genre.  
Only a basic example file was included with MiB64.  
If you're interested in using this feature, see if someone has published a suitable file. See [Web Links](web_links.md).

---

These files are collectively known as the **INI files**, **settings files**, or **support files** (because they support the application, not the user).  
You can check which versions you're using and visit the authors' homepages (to look for updates) via `Help > About INI Files`.

---

## Official vs Unofficial Releases

A minority of releases will be **Official**, meaning they come from the authors or their nominated contributors.  
Others are **Unofficial**, which means they could be from anyone.

If you're unfamiliar with the technical details of how these files work, stick to Official releases for quality assurance.  
If you're confident, use whatever you wish—or create your own.

A badly written file could:

- Render previously working games unplayable
- Crash the emulator
- Provide incorrect feedback

It cannot damage your system (they're plain text and cannot carry viruses).  
If in doubt, revert to the original files included with the emulator or the latest official ones.  
See [Web Links](web_links.md) for download locations.

---

## Installing INI Files

To install:

1. Download and extract/copy the file to the `MiB64 - 1.0\Config` folder.
2. Overwrite the existing file (if present).
3. Backup the original file by renaming it before you begin.

---

## Installing Updated Plugins

[Install updated plugins](additional_plugins.md) the same way you would add any plugin to MiB64.

- Usually the updated plugin will overwrite the older one.
- If you don't want this to happen, rename either version.
- Check the authors' documentation to see if two versions can be used concurrently, or if the old version must be uninstalled first.

---

**N.B.** Make sure all files you install are designed for your version of MiB64.  
Using older or newer versions could cause severe problems and must be avoided.

Before installing any file:

- Compare the version number with the one you're currently using via `Help > About INI Files`.
- After updating, confirm the new file is being used via `Help > About INI Files`.

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Updating Files Protocol Complete -->
