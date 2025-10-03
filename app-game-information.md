---
title: Game Information
nav_order: 7
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

## <center>Configuring Game Information</center>
<b>
<div style="text-align: center;">
  <div class="zoom-pair">
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
    </div>
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/game_information.png" alt="Game Information Dialog" width="155" />
    </div>
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Images -->

This tab is only available if [Hide Advanced Settings](app_options) is unchecked!

---

Options → Settings → Game Information

---

### Controls Available

1. <a name="o1">Game Status</a> (drop-down menu)  
2. <a name="o2">Players</a> (drop-down menu)  
3. <a name="o3">Force Feedback</a> (drop-down menu)  
4. <a name="o4">Core Note</a> (text box)  
5. <a name="o5">Plugin Note</a> (text box)  
6. <a name="o6">Game Language</a> (text box)  
7. <a name="o7">User Note</a> (text box)

---

### Points

- Changes made here affect the MiB64 Game Database Settings (`MiB64.rds`)  
- You may edit this file directly in a text editor (advanced users only)  
- To restore defaults, replace `MiB64.rdb` from the original archive  
- There is no “reset to defaults” button

---

### Field Descriptions

**<a name="o1">Game Status</a>**  
Drop-down menu listing all status categories from the RDS. To add/edit, modify the RDS manually.

**<a name="o2">Players</a>**  
Drop-down menu showing supported player counts from the RDI. To add/edit, modify the RDI manually.

**<a name="o3">Force Feedback</a>**  
Drop-down menu with Yes/No for rumble support.

**<a name="o4">Core Note</a>**  
Text field editing `Core Note=` for the current game in the RDS.

**<a name="o5">Plugin Note</a>**  
Text field editing `Plugin Note=` for the current game in the RDS.

**<a name="o6">Game Language</a>**  
Text field editing `GameLanguage=` in the RDI. Recommended format: English, French, German, etc.

**<a name="o7">User Note</a>**  
Text field for personal notes stored in the RDN. Displayed in the Game Browser if enabled.

> You must refresh the Game Browser for changes to take effect.

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
    <td style="text-align: center;">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Game Information Node Complete -->
