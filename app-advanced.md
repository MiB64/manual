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

<p style="text-align: center;">This tab is only available if <a href="app-options">Hide Advanced Settings</a> is unchecked!</p>

---

Options → Settings → Advanced

---

### <a name="Upper_tab"></a>Upper Tab – Core Defaults (drop-down menus)

1. [CPU core style](#b1)  
2. [Self-mod code method](#b2)  
3. [Advanced Block Linking](#b3)

---

## <a name="b1"></a>CPU Core Style

- Default: Recompiler  
- Recommended: Recompiler  
- Can be overridden per-ROM via [ROM Settings](app_rom_settings)  
- Interpreter may cause compatibility issues  
- MiB64 was tested primarily with Recompiler; Interpreter is fallback only

---

## <a name="b2"></a>Self-mod Code Method

- Default: Check Memory Advance  
- Recommended: Check Memory Advance  
- Usually set by RDS; rarely adjusted manually  
- Can be overridden per-ROM via [ROM Settings](app_rom_settings)  
- If RDS author couldn’t determine the correct value, manual adjustment may be needed

---

## <a name="b3"></a>Advanced Block Linking

- Default: On  
- Recommended: Off unless speed is needed  
- On = faster but less smooth  
- Off = smoother but slower  
- Most noticeable in racing games  
- Not normally set by RDS—this control is usually active  
- Introduced as toggle in MiB64 v1.4+

---

### <a name="Lower_tab"></a>Lower Tab – Checkboxes

1. [Start emulation when ROM is opened](#o1)  
2. [Automatically compress instant saves](#o2)  
3. [Clear Memory at Start Of Emulation](#o3)  
4. [Enable Debugger (forces CPU Interpreter)](#o4)  
5. [Show More Error Messages](#o5)

---

## <a name="o1"></a>Start Emulation When ROM Is Opened

- Default: Enabled  
- Recommended: Enabled  
- If disabled, allows editing ROM settings before boot  
- Saves you from manually starting emulation each time  
- Changes take effect at next ROM boot

---

## <a name="o2"></a>Automatically Compress Instant Saves

- Default: Enabled  
- Recommended: Enabled  
- Compresses state saves to reduce disk usage  
- No effect on loading saves  
- Compression level is fixed  
- Native saves are not compressed

---

## <a name="o3"></a>Clear Memory at Start Of Emulation

- Default: Enabled  
- Recommended: Enabled  
- Clears memory on each ROM load to prevent leftover junk  
- Prevents graphical glitches and data residue

---

## <a name="o4"></a>Enable Debugger (forces CPU Interpreter)

- Default: Disabled  
- Recommended: Disabled  
- Enables debugging mode using Interpreter (slower)  
- Previously required registry hacks; now exposed for advanced users  
- When enabled, performance drops significantly

---

## <a name="o5"></a>Show More Error Messages

- Default: Disabled  
- Recommended: Disabled  
- Displays additional debug messages when enabled  
- Useful for plugin developers or advanced troubleshooting

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

<!-- ClauseEcho: app_advanced.md Anchor Fidelity Restored -->
