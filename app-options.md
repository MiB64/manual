---
title: Options
nav_order: 4
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

# Configuration: Options

<div class="zoom-pair">
  <div class="zoom-on-hover">
    <img src="/manual/assets/images/config-settings.png" alt="Config Settings Dialog" width="300" height="207" />
  </div>
  <div class="zoom-on-hover">
    <img src="/manual/assets/images/app-options-defuult.png" alt="Options Dialog" width="155" />
  </div>
</div>
<p><strong>Hover to zoom</strong></p>

Options → Settings → Options

---

## Available Options

1. ["Pause emulation when window is not active"](#o1)
2. ["On loading a ROM go to full screen"](#o2)
3. ["Remember selected cheats"](#o3)
4. ["Disable AboutBox Audio"](#o4)
5. ["Hide Advanced Settings"](#o5)

---

## <a name="o1"></a>"Pause emulation when window is not active"

- Default: Enabled  
- Recommended: User preference

If enabled, MiB64 pauses when it loses focus.  
Useful for multitasking.

If disabled, MiB64 continues running in the background.  
Performance may drop while unfocused—this is normal.

---

## <a name="o2"></a>"On loading a ROM go to full screen"

- Default: Disabled  
- Recommended: Disabled

If enabled, MiB64 switches to fullscreen after loading a ROM.  
Useful if you know the game works and don’t need to adjust settings.

If disabled, games start windowed.  
Recommended so you can verify configuration before playing.

**Notes:**

- Fullscreen occurs *before* emulation starts—required for some plugins/hardware.
- Don’t enable this if “Start emulation after ROMs are opened” ([Advanced](app-advanced.md#o1)) is disabled.
- The RDB may override this for games marked “Unsupported.”  
  You can edit the RDB or change the game’s status if needed.

---

## <a name="o3"></a>"Remember selected cheats"

- Default: Disabled  
- Recommended: Disabled

If enabled, MiB64 remembers your cheat selections between sessions.  
Useful for convenience, but may cause strange behavior if forgotten.

If disabled, cheat selections reset when loading a new ROM or quitting.  
Recommended due to cheat instability.

---

## <a name="o4"></a>"Disable AboutBox Audio"

- Default: Disabled  
- Recommended: User preference

If enabled, MiB64’s “Epic Music” will not play.  
If disabled, it will play in full glory.  
This is purely a personal choice.

---

## <a name="o5"></a>"Hide Advanced Settings"

- Default: Enabled  
- Recommended: Enabled for beginners, disabled for advanced users

New in v1.5. When enabled, most advanced controls are hidden.  
Prevents confusion and misconfiguration.

Recommended for:

- New users
- Low technical expertise
- Young children

MiB64 runs equally well with this on or off.

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Options Configuration Protocol Complete -->
