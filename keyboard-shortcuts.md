---
title: Keyboard Shortcuts
nav_order: 6
parent: Using MiB64
---

<style>
.zoom-pair {
  display: flex;
  gap: 12px;
  align-items: flex-start;
  position: relative;
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

## <center><b>Keyboard Shortcuts</b></center>
<b>
<div style="text-align: center;">
<div class="zoom-on-hover">
  <img src="/manual/asset/images/main.png" alt="MiB64 Main Browser" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

This section will take you through keyboard shortcuts in MiB64.

### Notes:

1. The shortcut keys available to you depend on the state of the emulator (mirrors availability of the associated menu items).
2. Remember you can also navigate the menus with the ALT+(key) indicators, e.g. by default ALT+F opens the file menu, then pressing S would Start Emulation (these keys are set up by the language file so they depend on the file and your current language selection).
3. Note that CTRL+ key combinations open dialogues while F(function) keys have instant effects. F-key shortcuts are available while fullscreen but CTRL+keys are not.
4. You cannot change the shortcut keys in MiB64 (but if you have a gamepad with lots of buttons and good software you could map to those).

### Available in browser and during emulation:

| Action                          | Shortcut     |
|:---------------------------------|:-------------|
| open Game dialog                 | CTRL+O       |
| settings dialog                  | CTRL+T       |
| quit application                 | ALT+F4       |
| start emulation                  | F10          |
| end emulation                    | F11          |

### Available only during emulation:

| Action                          | Shortcut     |
|:---------------------------------|:-------------|
| switch fullscreen/windowed       | ALT+ENTER / Escape |
| reboot Game                      | F1           |
| pause/resume emulation           | F2           |
| generate bitmap                  | F3*          |
| enable/disable speed limiter     | F4*          |
| state quick save                 | F5           |
| state save dialog                | CTRL+S       |
| state quick load                 | F7           |
| state load dialog                | CTRL+L       |
| select quick state save slot     | 0–9          |
| game details (name, size etc)    | CTRL+I       |
| game information (GDX Game Page) | CTRL+G       |
| always on top toggle             | CTRL+A       |
| cheat dialog                     | CTRL+C       |
| cheat search                     | CTRL+R       |
| configure graphics plugin        | CTRL+V       |
| configure audio plugin           | CTRL+U       |
| configure rsp plugin             | CTRL+W       |
| configure settings               | CTRL+T       |
| gs button (gameshark button)     | F9           |

### Available only in Game Browser:

| Action                          | Shortcut     |
|:---------------------------------|:-------------|
| refresh                          | F5           |
| jump to top                      | Home         |
| jump to bottom                   | End          |
| up one page                      | Page Up      |
| down one page                    | Page Down    |
| up one line                      | Up arrow     |
| down one line                    | Down arrow   |
| jump to Game starting with...    | 0–9 A–Z      |
| start selected game              | Enter        |
| open menu                        | right mouse button |
| edit cheats                      | right mouse button* |

*only available in Advanced mode.

---

<!-- Footer Navigation Block -->

<table align="center" style="width: 80%">
  <tr>
    <td style="text-align: center"><a href="using-mib64">Using MiB64</a></td>
    <td style="text-align: center"><a href="start-stop-reset-games">Start, Stop, Reset Games</a></td>
    <td style="text-align: center"><a href="save-load-games">Save & Load Games</a></td>
    <td style="text-align: center"><a href="/manual/manual/manual/cheats">Using Cheats</a></td>
  </tr>
  <tr>
    <td style="text-align: center"><a href="taking-screenshots">Taking Screenshots</a></td>
    <td style="text-align: center"><a href="multiple-instances">Multiple Instances</a></td>
    <td style="text-align: center"><a href="keyboard-shortcuts">Keyboard Shortcuts</a></td>
    <td style="text-align: center"><a href="using-mib64-troubleshooting-stability">Troubleshooting Stability</a></td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Shortcut Protocol Activated -->
