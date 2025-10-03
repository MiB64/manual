---
title: Advanced
nav_order: 5
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

## <center>Configuration: Advanced</center>
<b>
<div style="text-align: center;">
  <div class="zoom-pair">
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
    </div>
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/advanced.png" alt="Advanced Dialog" width="155" />
    </div>
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Images -->

This tab is only available if [Hide Advanced Settings](app_options) is unchecked!

---

Options → Settings → Advanced

---

### <a name="Upper_tab">Upper tab – Core Defaults (drop-down menus)</a>

1. <a name="b1">CPU core style</a>  
2. <a name="b2">Self-mod code method</a>  
3. <a name="Advanced_Block_Linking">Advanced Block Linking</a> ← Important control, read this!

---

#### <a name="b1">CPU core style</a>

- Default: Recompiler  
- Recommended: Recompiler (should not matter if using RDS)  
- Can be overridden per-ROM via [ROM Settings](app_rom_settings) if RDS is enabled  
- MiB64 was tested primarily with Recompiler; Interpreter may cause issues

---

#### <a name="b2">Self-mod code method</a>

- Default: Check Memory Advance  
- Recommended: Same  
- Usually set by RDS; rarely adjusted manually  
- Can be overridden per-ROM via [ROM Settings](app_rom_settings)

---

#### <a name="Advanced_Block_Linking">Advanced Block Linking</a>

- Default: On  
- Recommended: Off (unless speed is needed)  
- Affects recompiler performance:  
  - On = faster but less smooth  
  - Off = smoother but slower  
- Most noticeable in racing games  
- Not normally set by RDS—this control is usually active

---

### <a name="Lower_tab">Lower tab – Checkboxes</a>

1. <a name="o1">Start emulation when ROM is opened</a>  
2. <a name="o2">Automatically compress instant saves</a>  
3. <a name="o3">Clear Memory at Start Of Emulation</a>  
4. <a name="o4">Enable Debugger (forces CPU Interpreter)</a>  
5. <a name="o5">Show More Error Messages</a>

---

#### <a name="o1">Start emulation when ROM is opened</a>

- Default: Enabled  
- Recommended: Enabled  
- If disabled, allows editing ROM settings before boot  
- Changes take effect at next ROM boot

---

#### <a name="o2">Automatically compress instant saves</a>

- Default: Enabled  
- Recommended: Enabled  
- Compresses state saves to reduce disk usage  
- No effect on loading saves  
- Compression level is fixed  
- Native saves are not compressed

---

#### <a name="o3">Clear Memory at Start Of Emulation</a>

- Default: Enabled  
- Recommended: Enabled  
- Clears memory on each ROM load to prevent leftover junk

---

#### <a name="o4">Enable Debugger (forces CPU Interpreter)</a>

- Default: Disabled  
- Recommended: Disabled  
- Enables debugging mode using Interpreter (slower)  
- Previously required registry hacks; now exposed for advanced users

---

#### <a name="o5">Show More Error Messages</a>

- Default: Disabled  
- Recommended: Disabled  
- Displays additional debug messages when enabled

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

<!-- ClauseEcho: Advanced Node Complete -->
