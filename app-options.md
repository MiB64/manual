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

- default setting: enabled  
- generally recommended setting: user preference!

If enabled, the emulator will pause when it detects that it no longer has focus in Windows. This is useful if you are multitasking and want the emulator to pause whenever you go to another application.

If disabled, the emulator will carry on running regardless of whether or not it has focus. Use this if you want MiB64 to carry on running in the background while you do something else (you can still keep it always on top with the Always on Top option!). Note that if this option is unchecked the peformance of MiB64 will probably be lower while focus is lost because of the way Windows handles resources. This is normal and not a fault of MiB64.

---

### <a name="o2"></a>“On loading a ROM go to full screen”

- default setting: disabled  
- generally recommended setting: disabled

If enabled, MiB64 will automatically instruct the video plugin to switch to fullscreen once after loading each ROM. This is good (saves you a key press) if you know a game works and doesn't need any configuration changes. You can still return to windowed mode in the usual ways (Escape, ALT+ENTER).

If disabled, games will start windowed. You can switch to fullscreen mode yourself in the usuall ways (Escape, ALT+ENTER, Options menu). This is a little more work (one key press) but recommended, because you can make sure your configuration (particularly graphics plugin tabs) is correct before getting into your game.

**Notes:**

- The emulator actually goes fullscreen *before* starting emulation. This is so that plugins/hardware that *only* work in fullscreen can be supported. If you have such a plugin or hardware then you *must* enable this option!
- Don't enable this option with "Start emulation after ROMs are opened" ([Advanced](app_advanced.html)) disabled! It will go fullscreen but you your games won't start, which could be confusing...
- The RDB can override this option and prevent automatic fullscreen on a defined status (by default, games with status "Unsupported"). Hopefully it's obvious why this is done; if you don't like it you can either edit the RDB to remove the line from the status definition, or you could change the status of the game(s).

---

### <a name="o3"></a>“Remember selected cheats”

- default setting: Enabled  
- generally recommended setting: user preference.

If enabled, MiB64 will save your cheat code selection between sessions. This is for your convenience, and it means that if you close the emulator and go away, then play some hours/weeks/anytime later, the same cheat codes will be applied as before... this is important to keep in mind if your games are acting strangely!

If disabled, the cheat code selection is lost as soon as you load a new ROM, or quit the application, whichever happens first. This is recommended because cheat codes tend to cause problems...

---

### <a name="o4"></a>“Disable AboutBox Audio”

- default setting: disabled  
- generally recommended setting: user preference

If enabled, The MiB64 'Epic Music' will not play! This option is available as a user preference to enable / disable the audio in any way they wish to ....

If disabled, The MiB64 'Epic Music' will play in all its glory! This option again is available as a user preference to enable / disable the audio in any way they wish to ....

---

### <a name="o5"></a>“Hide Advanced Settings”

- default setting: disabled 
- generally recommended setting: user preference.

When enabled, most of MiB64's other controls are hidden from the user. This is because casual fiddling by inexperienced users tends to result in people getting themselves into a mess. It is therefore highly recommended that new users, people with low technical/emulator expertise, and young children, to give a few examples, use the application with this option enabled - the emulator runs just as well will this on or off!

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

<!-- ClauseEcho: Options Node Complete -->
