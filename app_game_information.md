---
title: Game Information
nav_order: 8
parent: Application Settings
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

# Configuring Game Information

<div class="zoom-pair">
  <div class="zoom-on-hover">
    <img src="/manual/assets/images/config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
  </div>
  <div class="zoom-on-hover">
    <img src="/manual/assets/images/game_information.png" alt="Game Information Dialog" width="155" />
  </div>
</div>
<p><strong>Hover to zoom</strong></p>

Options → Settings → Game Information

---

**Note:** This tab is only available if [Hide Advanced Settings](app_options.md#o5) is unchecked.

---

## Controls Available

1. [Game Status](#o1) (drop-down menu)  
2. [Players](#o2) (drop-down menu)  
3. [Force Feedback](#o3) (drop-down menu)  
4. [Core Note](#o4) (text box)  
5. [Plugin Note](#o5) (text box)  
6. [Game Language](#o6) (text box)  
7. [User Note](#o7) (text box)

---

## Points

- Changes here edit the MiB64 Game Database Settings (`MiB64.rds`)  
- You may also edit the file directly in a text editor (advanced users only)  
- There is no “reset to defaults” button—restore by replacing `MiB64.rds` from the original archive

---

### <a name="o1"></a>"Game Status"

Drop-down menu listing all status categories from the RDS.  
To add or edit categories, manually edit the RDS file.

---

### <a name="o2"></a>"Players"

Drop-down menu listing supported player counts from the RDI.  
To add or edit categories, manually edit the RDI file.

---

### <a name="o3"></a>"Force Feedback"

Drop-down menu with Yes/No options for Rumble support.

---

### <a name="o4"></a>"Core Note"

Text field that edits the `Core Note=` line for the current game in the RDS.

---

### <a name="o5"></a>"Plugin Note"

Text field that edits the `Plugin Note=` line for the current game in the RDS.

---

### <a name="o6"></a>"Game Language"

Text field that edits the `GameLanguage=` line for the current game in the RDI.  
Recommended format: English, French, German, etc.

---

### <a name="o7"></a>"User Note"

Text field that adds and displays a personal `User Note` for the current game in the RDN.  
Used for personal notes in the Game Browser.

---

You must refresh the Game Browser for any changes to take effect.

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Game Information Protocol Complete -->
