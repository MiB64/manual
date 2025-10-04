---
title: Using MiB64
nav_order: 12
---

<!-- This one is the best to use for all situations. -->        
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
  position: relative;
  z-index: 1;
  transform-origin: left center;
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

/* Final fix for standalone zoomable images */
.zoom-single {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: max-content;
  text-align: center;
}

.zoom-single:hover img {
  transform: scale(1.5);
  transform-origin: center center;
  z-index: 999;
}
</style>

## <center><b>Using MiB64</b></center>
<b>    
<div style="text-align: center;">
<div class="zoom-on-hover">
  <img src="/manual/asset/images/main.png" alt="MiB64 Main Browser" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

<a name="Main_window"></a>
## <center><b>Main Window</b></center>
<b>

Should be straightforward enough—starting from the top:

- Title bar shows the internal name of the loaded game, followed by the app title and version number.  
- Minimize, maximize (only in Game Browser), and exit buttons.  
- **File menu**: Game loading, Start/End emulation, language selection.  
- **System menu**: Available while emulator is running.  
- **Options menu**: Access to main settings dialog and plugin selection.  
- **Help menu**: Documentation and About info.  
- **Status bar** (lower left): Emulator state feedback and optional CPU load stats.  
- **FPS counter** (bottom right): Displays VI/s (Fields Per Second) of the CPU core—not graphics FPS.

---

<a name="Game_Browser"></a>
## <center><b>Using the Game Browser</b></center>
<b>

### Navigation Links:
- [Status and colour coding](#status)  
- [Notes fields](#notes)  
- [Navigation, Sorting, Configuration](#navigation)

### Points:
1. The Game Browser does not verify your games! You **must** use a separate verification utility—MiB64 recommends [Verifying Games](verify-games).  
2. “Good Name” is a field in the RDS, not a verification method.  
3. Games are identified by CRC pairs and country code. Bad games with matching codes may appear as good.  
4. Status, colours, and notes come from the RDS file (editable by advanced users).  
5. Games marked “Unknown” are likely bad or unverified.  
6. The Browser uses a cache file in the MiB64 root folder. Refresh manually if game folder contents change.

---

<a name="status"></a>
## <center><b>Status Colour Coding</b></center>
<b>

<p><font color="#006600">"Compatible" (green)<br>
The game is, to the best of our knowledge, fully playable, with no issues severe enough to seriously affect gameplay...
</font></p>

<p><font color="#827B00">"Issues (core)/Issues (plugin)" (muddy yellow)<br>
These games can be played, but they have moderate to severe issues...
</font></p>

<p><font color="#00897C">"Needs video plugin" (turquoise)<br>
These games are supported on the core but fail with default plugins...
</font></p>

<p><font color="#00897C">"Needs audio plugin" (turquoise)<br>
Same as above, but for audio. Rare.
</font></p>

<p><font color="#800080">"Use (named) plugin" (purple)<br>
Indicates the best plugin for this game.
</font></p>

<p><font color="#990000">"Unsupported" (dark red)<br>
Known to fail on the core. No plugin or setting will help.
</font></p>

<p><font color="#603913">"Broken (core)/Broken (plugin)" (brown)<br>
Use older MiB64 version or plugin. See Notes.
</font></p>

<p><font color="#000099">"Region issue" (blue)<br>
Another version of the game works. Read the note.
</font></p>

<p><font color="#003300">"Interpreter only" (medium green)<br>
Game only runs on interpreter core.
</font></p>

<p>"Uncertain" (black)<br>
Status unknown—test manually.
</p>

<p><font color="#444444">"Unknown" (grey)<br>
Not found in RDS or no status defined. Likely a bad or unverified Game.
</font></p>

---

<a name="notes"></a>
## <center><b>Notes Fields</b></center>
<b>

Notes are split into core and plugin fields to reflect separate compatibility layers.

Keep in mind:
- Most text explains known issues.  
- Instructions often begin with “use…”—follow them.  
- Complex notes may refer you to the GameFAQ (accessible via Help menu).

### Abbreviations:
- `:` means “for” → e.g. `Framebuffer:flare` = “enable Framebuffer for flare”  
- `;` means “therefore” → e.g. `doesn't start; use PAL version` = “game doesn’t start, so use PAL version”

### Common Shortforms:
- `"res."` = resolution  
- `"v."` or `"ver"` = version  
- `(E)`, `(U)` etc. = GoodN64 country codes  
- `"NTSC"` = US, Japan, etc.  
- `"PAL"` = Europe, Australia, etc.  
- `"?"` = RDS author was unsure

---

<a name="navigation"></a>
## <center><b>Game Browser Navigation</b></center>
<b>

- Use mouse (scroll bars, wheel, buttons) or [shortcut keys](keyboard-shortcuts) for faster navigation.  
- Click column headers to sort—click again to reverse direction.  
- The browser is highly [configurable](#Game_Browser).

---

<!-- Footer Navigation Block -->

<table align="center" style="width: 80%">
  <tr>
    <td style="text-align: center"><a href="using-mib64">Using MiB64</a></td>
    <td style="text-align: center"><a href="start-stop-reset-games">Start, Stop, Reset Games</a></td>
    <td style="text-align: center"><a href="save-load-games">Save &amp; Load Games</a></td>
    <td style="text-align: center"><a href="cheats">Using Cheats</a></td>
  </tr>
  <tr>
    <td style="text-align: center"><a href="taking-screenshots">Taking Screenshots</a></td>
    <td style="text-align: center"><a href="multiple-instances">Multiple Instances</a></td>
    <td style="text-align: center"><a href="keyboard-shortcuts">Keyboard Shortcuts</a></td>
    <td style="text-align: center"><a href="using-mib64-troubleshooting-stability">Troubleshooting Stability</a></td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Using MiB64 Protocol Activated -->
