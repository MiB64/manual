---
title: Directories
nav_order: 2
parent: Settings (Application)
---

<style>
.zoom-pair {
  display: flex;
  gap: 12px;
  align-items: flex-end;
  justify-content: flex-start;
  position: relative;
  margin-left: auto;
  margin-right: auto;
  width: max-content;
  text-align: left;
}

.zoom-on-hover {
  display: inline-block;
  position: relative;
}

.zoom-on-hover img {
  display: block;
  cursor: zoom-in;
  transition: transform 0.3s ease;
  transform-origin: left center;
  position: relative;
  z-index: 1;
}

.zoom-on-hover:hover img {
  transform: scale(1.5);
}

.zoom-pair .zoom-on-hover:first-child:hover img {
  z-index: 9999;
}

.zoom-pair .zoom-on-hover:last-child:hover img {
  z-index: 100;
}
</style>

## <center>Configuration: Directories</center>
<b>
<div style="text-align: center;">
  <div class="zoom-pair">
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
    </div>
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/directories.png" alt="Directories Dialog" width="155" />
    </div>
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Images -->

Options → Settings → Directories

---

N.B. It is purely a matter of personal preference how you set these folders,  
but you *must* have the Plugin folder set correctly for MiB64 to start up properly.  
If valid plugins aren't found at the configured path when MiB64 starts, you cannot launch games.

This is by design—plugins are essential.  
You can still access Options to correct the paths.

---

## Folder Types

MiB64 allows you to configure up to five directories:

1. **Plugin Directory**  
   All plugins must be placed together in one folder.  
   Default: `\Plugin\` subfolder of the main MiB64 folder.

2. **Game Directory**  
   MiB64 remembers the last used folder by default.  
   You can force it to always use a specific folder.

3. **N64 Native Saves Directory**  
   All native save types will be placed here.  
   Default: `\Save\` subfolder of the main MiB64 folder.

4. **Quick Save States Folder**  
   All state slot files will be placed here.  
   Default: same folder as native saves.

5. **Screenshots Directory**  
   Used by the video plugin for screenshots.  
   Default: `\Screenshots\` subfolder of the main MiB64 folder.

---

Each folder can use either a default path or a custom one.  
You can type a path directly or browse using the “...” button.  
Press OK to confirm and save your changes.

---

<table align="center">
  <tr>
    <td style="text-align: center;"><a href="app_settings">Settings</a></td>
    <td style="text-align: center;"><a href="app_plugins">Plugins</a></td>
    <td style="text-align: center;"><a href="app_directories">Directories</a></td>
    <td style="text-align: center;"><a href="app_options">Options</a></td>
    <td style="text-align: center;"><a href="app_game_selection">Game Selection</a></td>
  </tr>
  <tr>
    <td style="text-align: center;"><a href="app_advanced">Advanced</a></td>
    <td style="text-align: center;"><a href="app_game_settings">Game Settings</a></td>
    <td style="text-align: center;"><a href="app_game_information">Game Information</a></td>
    <td style="text-align: center;"><a href="app_language">Language Selection</a></td>
    <td style="text-align: center;">&nbsp;</td> <!-- Empty cell for symmetry -->
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Directories Node Complete -->
