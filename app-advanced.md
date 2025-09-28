---
title: Advanced
nav_order: 6
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

# Configuration: Advanced

<div class="zoom-pair">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images//config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
  </div>
  <div class="zoom-on-hover">
    <img src="/manual/asset/images//advanced.png" alt="Advanced Dialog" width="155" />
  </div>
</div>
<p><strong>Hover to zoom</strong></p>

Options → Settings → Advanced

---

**Note:** This tab is only available if [Hide Advanced Settings](app_options.md#o5) is unchecked.

---

## <a name="Upper_tab"></a>Upper Tab – Core Defaults (Dropdowns)

### <a name="b1"></a>"CPU core style"

- Default: Recompiler  
- Recommended: Recompiler (should not matter if using RDS)

Can be overridden per-ROM via [ROM Settings](app_game_settings.md#o1) if RDS is enabled.  
MiB64 was tested primarily with Recompiler. Interpreter may cause issues in some games.

---

### <a name="b2"></a>"Self-mod code method"

- Default: Check Memory Advance  
- Recommended: Check Memory Advance (should not matter if using RDS)

Also overridden via [ROM Settings](app_game_settings.md#r1) if RDS is enabled.  
Usually set by the RDS author. If not, you may need to determine the correct value manually.

---

### <a name="b3"></a>"Advanced Block Linking"

- Default: On  
- Recommended: Off (unless you need speed)

ABL is a speed optimization for the recompiler.  
- On = higher speed, more variation  
- Off = smoother performance, less variation

Most noticeable in racing games like Diddy Kong Racing and Mario Kart.

Can be overridden via [ROM Settings](app_game_settings.md#r2) if RDS is enabled.  
MiB64 was tested with ABL enabled. Turning it off may require adjusting other settings.

**Notes:**

- Some games may not work with ABL off—be prepared to re-enable it per-ROM.
- ABL was always present in MiB64; version 1.4+ simply lets you disable it.

---

## <a name="Lower_tab"></a>Lower Tab – Checkboxes

### <a name="o1"></a>"Start emulation after ROMs are opened"

- Default: Enabled  
- Recommended: Enabled (unless you want to edit RDS before boot)

If enabled, emulation starts immediately after ROM load.  
If disabled, you must manually start emulation—useful for editing settings before boot.

Changes take effect on next ROM boot.

---

### <a name="o2"></a>"Automatically compress instant saves"

- Default: Enabled  
- Recommended: Enabled

If enabled, state saves are compressed (Slots and Save As).  
Saves space but may take longer to complete.

If disabled, saves are uncompressed—faster but larger (4MB or 8MB depending on Expansion Pak).

**Notes:**

- Loading is unaffected—you can load compressed saves even if disabled.
- Compression level is fixed.
- Native saves are not compressed (too small to justify).

Changes take effect immediately or on next save.

---

### <a name="o3"></a>"Clear Memory at Start Of Emulation"

- Default: Enabled  
- Recommended: Enabled

Clears memory on every new ROM load.  
Older versions left junk in memory—this prevents that.

---

### <a name="o4"></a>"Enable Debugger (forces CPU Interpreter)"

- Default: Disabled  
- Recommended: Disabled

Previously required a registry file and debug build.  
Now available directly for advanced users.

When enabled, emulator runs in interpreter mode—much slower.

---

### <a name="o5"></a>"Show More Error Messages"

- Default: Disabled  
- Recommended: Disabled

Displays additional error messages in debug mode.

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Advanced Configuration Protocol Complete -->
