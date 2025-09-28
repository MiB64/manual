---
title: Game Settings
nav_order: 7
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

# Configuring Game Settings

<div class="zoom-pair">
  <div class="zoom-on-hover">
    <img src="/manual/assets/images/config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
  </div>
  <div class="zoom-on-hover">
    <img src="/manual/assets/images/game_settings.png" alt="Game Settings Dialog" width="155" />
  </div>
</div>
<p><strong>Hover to zoom</strong></p>

Options → Settings → <a name="ROM_Settings">ROM Settings</a>

---

**Note:** This tab is only available if [Hide Advanced Settings](app_options.md#o5) is unchecked.

This page configures the core for each individual ROM.  
Some settings also appear under the General tab, but here they apply per-ROM.

---

## Sections

- [General Settings](#General_Settings)
- [Recompiler Settings](#Recompiler_Settings)

---

## <a name="General_Settings"></a>General Settings

### <a name="o1"></a>"CPU core style"

- Options: *use general setting, Interpreter, Recompiler, Synchronise Cores (debug only)  
- Default: *use general setting (Recompiler)  
- Recommended: Recompiler if stable

Recompiler = faster, less compatible  
Interpreter = slower, more compatible

If using Interpreter, the following are ignored:

- [Self-mod code method](#r1)  
- [Advanced Block Linking](#r2)  
- [Larger Compiler Buffer](#r3)  
- [Register Caching](#r5)

---

### <a name="o2"></a>"Memory size"

- Options: *use general setting, 4MB, 8MB  
- Default: *use general setting (8MB)  
- Recommended: 4MB unless required

8MB = Expansion Pak.  
Most games don’t benefit and may suffer performance or aspect ratio issues.  
Some games require it (e.g. Zelda2), others use it optionally (e.g. Perfect Dark).

---

### <a name="o3"></a>"Default save type"

- Options: *detect first used type, 4kbit EEPROM, 16kbit EEPROM, 32kbyte SRAM, 128kbyte FlashRAM  
- Default: *detect first used type  
- Recommended: *detect, unless game uses 16kbit EEPROM or copy protection

MemPak works in addition to this setting.

---

### <a name="o4"></a>"Counter Factor"

- Options: *use default (2), 1–6  
- Default: *use default (2)  
- Recommended: 1 or 2 (possibly 3)

Controls core timing.  
- 2 = best speed without issues  
- 1 = prevents flicker, improves smoothness  
- 3 = may improve performance  
- >3 = likely unstable

---

### <a name="o5"></a>"Vertical Interrupts per Second"

- Default: 1500  
- Recommended: 1500 unless required

Controls emulated refresh rate.  
Originally locked, now user-accessible.

---

### <a name="o6"></a>"Emulate AI"

- Default: Unchecked  
- Recommended: Unchecked unless needed

Added in v1.6.1 to fix sound/speech issues in games like Hydro Thunder, Tarzan, Top Gear Rally, RE2, TWINE.

---

### <a name="o7"></a>"Use TLB"

- Default: Checked  
- Recommended: Checked if needed, unchecked otherwise

Required by some games (e.g. Goldeneye, Mario).  
Disabling may improve performance if not needed.

---

### <a name="o8"></a>"RSP Audio Signal"

- Default: Unchecked  
- Recommended: Unchecked unless needed

Enables Musyx support for games like Hydro Thunder, NBA Showtime, Tarzan, TWINE, RE2.

---

### <a name="o9"></a>"Delay SI interrupt"

- Default: Unchecked  
- Recommended: Unchecked unless needed

Added in v1.5 to fix broken games from v1.4 (e.g. Cruis'N USA).  
Usually not required.

---

## <a name="Recopiler_Settings"></a>Recompiler Settings

### <a name="r1"></a>"Self-mod code method"

- Options: *use general setting, None, Cache, Check Memory & Cache, Check Memory Advance, Change Memory & Cache, Protect Memory  
- Default: *use general setting (Check Memory Advance)  
- Recommended: Game-dependent

Used to handle games with self-modifying code.  
Methods range from fast to secure:

`None < Cache < Check Memory & Cache < Check Memory Advance < Change Memory & Cache < Protect Memory`

---

### <a name="r2"></a>"Advanced Block Linking"

- Options: *use general setting, Off, On  
- Default: *use general setting (On)  
- Recommended: Game-dependent

Speed vs. smoothness tradeoff.  
On = faster, Off = smoother.  
Some games require specific setting.

---

### <a name="r3"></a>"Larger Compiler Buffer"

- Default: Unchecked  
- Recommended: Unchecked unless needed

Increases buffer from 20MB to 50MB.  
Helps games with complex code structures.  
Most games don’t need it.

---

### <a name="r4"></a>"SP Hack"

- Default: Unchecked  
- Recommended: Unchecked

Added in v1.5 for performance.  
May give 5% speed boost but causes instability in many games.

---

### <a name="r5"></a>"Register Caching"

- Default: Checked  
- Recommended: Checked unless unstable

Major optimization.  
Can cause obscure errors—disable if recompiler is unstable.

---

### <a name="r7"></a>"Unalign DMA"

- Default: Unchecked  
- Recommended: Unchecked unless using old SM64 ROM hacks

Supports faulty alignment in old hacks.  
Should be off for normal games.

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Game Settings Protocol Complete -->
