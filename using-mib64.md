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

<div class="zoom-single">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/browser.png" alt="Main Browser Window" width="380" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>
<!-- ClauseEcho: Interactive Image -->

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

## <center><b>Status Colour Coding</b></center>
<b>

MiB64 uses “Status” instead of “Playable” to avoid subjective ambiguity. Status is a defined category in the RDS and determines row colour in the Game Browser.

- **Compatible** (green): Fully playable, no major issues.  
- **Issues (core/plugin/mixed)** (muddy yellow): Moderate to severe issues.  
- **Needs video plugin** (turquoise): Core may be fine, but default plugin fails.  
- **Needs audio plugin** (turquoise): Same as above, but for audio.  
- **Use (named) plugin** (purple): Specific plugin recommended.  
- **Unsupported** (dark red): Known to fail on MiB64 core.  
- **Broken (core/plugin)** (brown): Use older MiB64 version or plugin.  
- **Region issue** (blue): Another version of the game works.  
- **Interpreter only** (medium green): Game only runs on interpreter core.  
- **Uncertain** (black): Status unknown—test manually.  
- **Unknown** (grey): Not found in RDS or no status defined.

---

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

## <center><b>Game Browser Navigation</b></center>
<b>

- Use mouse (scroll bars, wheel, buttons) or [shortcut keys](keyboard_shortcuts) for faster navigation.  
- Click column headers to sort—click again to reverse direction.  
- The browser is highly [configurable](#ROM_Browser).

---

## <center><b>Navigation</b></center>
<b>

<table align="center" style="width: 80%">
  <tr>
    <td style="text-align: center"><a href="using_mib64.html">Using MiB64</a></td>
    <td style="text-align: center"><a href="start_stop_reset_games.html">Start, Stop, Reset Games</a></td>
    <td style="text-align: center"><a href="save_load_games.html">Save &amp; Load Games</a></td>
    <td style="text-align: center"><a href="/cheats/">Using Cheats</a></td>
  </tr>
  <tr>
    <td style="text-align: center"><a href="taking_screenshots.html">Taking Screenshots</a></td>
    <td style="text-align: center"><a href="multiple_instances.html">Multiple Instances</a></td>
    <td style="text-align: center"><a href="keyboard_shortcuts.html">Keyboard Shortcuts</a></td>
    <td style="text-align: center"><a href="using_mib64_troubleshooting_stability.html">Troubleshooting Stability</a></td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Using MiB64 Protocol Activated -->
