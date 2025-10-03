---
title: Options
nav_order: 3
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

## <center>Configuration: Options</center>
<b>
<div style="text-align: center;">
  <div class="zoom-pair">
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
    </div>
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/app_options_defuult.png" alt="Options Dialog" width="155" />
    </div>
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Images -->

Options → Settings → Options

---

## Option Toggles

1. [“Pause emulation when window is not active”](#o1)  
2. [“On loading a ROM go to full screen”](#o2)  
3. [“Remember selected cheats”](#o3)  
4. [“Disable AboutBox Audio”](#o4)  
5. [“Hide Advanced Settings”](#o5)

---

### <a name="o1"></a>“Pause emulation when window is not active”

- **Default:** Enabled  
- **Recommended:** User preference

If enabled, MiB64 pauses when it loses focus—ideal for multitasking.  
If disabled, it continues running in the background. Performance may drop when unfocused due to Windows resource handling.

---

### <a name="o2"></a>“On loading a ROM go to full screen”

- **Default:** Disabled  
- **Recommended:** Disabled

If enabled, MiB64 switches to fullscreen automatically after loading a ROM.  
If disabled, games start windowed and you manually toggle fullscreen.

**Notes:**

- Fullscreen activates *before* emulation starts—required for some plugins/hardware.  
- Avoid enabling this if “Start emulation after ROMs are opened” is disabled.  
- The RDB may override this setting for games marked “Unsupported.”

---

### <a name="o3"></a>“Remember selected cheats”

- **Default:** Disabled  
- **Recommended:** Disabled

If enabled, cheat selections persist across sessions.  
If disabled, cheat selections reset when loading a new ROM or quitting.  
Recommended to disable—cheats often cause instability.

---

### <a name="o4"></a>“Disable AboutBox Audio”

- **Default:** Disabled  
- **Recommended:** User preference

If enabled, MiB64’s “Epic Music” won’t play.  
If disabled, the music plays in full.  
This is purely aesthetic—choose freely.

---

### <a name="o5"></a>“Hide Advanced Settings”

- **Default:** Enabled  
- **Recommended:** Enabled for beginners; disabled for advanced users

Introduced in v1.5. When enabled, most advanced controls are hidden.  
Recommended for new users, children, or those unfamiliar with emulator settings.  
MiB64 runs identically with this on or off.

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
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Options Node Complete -->
