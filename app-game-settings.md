---
title: Game Settings
nav_order: 6
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

## <center>Configuring Game Settings</center>
<b>
<div style="text-align: center;">
  <div class="zoom-pair">
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
    </div>
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/game_settings.png" alt="Game Settings Dialog" width="155" />
    </div>
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Images -->

This tab is only available if [Hide Advanced Settings](app_options) is unchecked!

---

Options → Settings → ROM Settings

---

This page covers configuration of the core for each individual ROM. Some of these settings are also available under the General tab, but here they apply per-ROM.

---

### <a name="General_Settings">General Settings</a>

1. <a name="o1">CPU core style</a>  
2. <a name="o2">Memory size</a>  
3. <a name="o3">Default save type</a>  
4. <a name="o4">Counter Factor</a>  
5. <a name="o5">Vertical Interrupts per Second</a>  
6. <a name="o6">Emulate AI</a>  
7. <a name="o7">Use TLB</a>  
8. <a name="o8">RSP Audio Signal</a>  
9. <a name="o9">Delay SI interrupt</a>

---

### <a name="Recopiler_Settings">Recopiler Settings</a>

1. <a name="r1">Self-mod. code method</a>  
2. <a name="r2">Advanced Block Linking</a>  
3. <a name="r3">Larger Compiler Buffer</a>  
4. <a name="r4">SP Hack</a>  
5. <a name="r5">Register Caching</a>  
6. <a name="r7">Unalign DMA</a>

---

### Points

- Do not change these settings unless you fully understand them  
- Changes affect the MiB64 ROM Database (`MiB64.rds`)  
- To restore defaults, replace `MiB64.rds` from the original archive  
- No “reset to defaults” button exists

---

### Field Descriptions

Each setting includes default and recommended values, compatibility notes, and performance tradeoffs. Interpreter disables recompiler-only settings like `r1`, `r2`, `r3`, `r5`.

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

<!-- ClauseEcho: Game Settings Node Complete -->
