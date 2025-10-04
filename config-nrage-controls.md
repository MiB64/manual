---
title: Controls Config
nav_order: 1
parent: Input (Controller) Config
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
  position:relative;
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

## <center><b>N-Rage MiB64 Input Configuration — Controls Tab</b></center>
<b>

<div style="text-align: center;">
  <div class="zoom-single">
    <img src="/manual/asset/images/NRage_MiB64_Input_Controls.png" alt="Controls Tab" width="320" height="224" />
    <p><strong>Hover to zoom</strong></p>
  </div>
</div>

---

### <a name="basic-configuration"></a>Basic Configuration

At the bottom of the window, you'll find three buttons:

- **Save** — Stores all changes and closes the window.  
- **Use** — Temporarily applies settings while the emulator is running. Changes are lost if you reset, close the ROM, or load a save state.  
- **Cancel** — Discards all changes.

There's also a **language selector** dropdown. If you've installed a language pack, select your language, click Save, and reopen the configuration screen. No emulator restart is required.

---

### <a name="input-types"></a>DirectInput and XInput Support

- **DirectInput** is selected by default.  
- **Plugged** — Indicates whether the emulator sees the controller. Unchecked means no input is registered.  
- **Background Input** — Allows input even when the emulator window isn't focused.  
- **XInput** — Enables configuration for XInput-compatible controllers.  
- **N64 Mouse** — Enables N64 mouse support.

---

### <a name="profiles"></a>Profiles and Defaults

- **Clear Controller** — Unbinds all keys, modifiers, and settings.  
- **Default Config** — Restores default assignments, modifiers, and sliders. Does not erase mempak data.  
- **Load Profile** — Loads a `.cpf` file. Not compatible with versions ≤1.83. Ensure devices are plugged in before loading.  
- **Save Profile** — Saves current configuration to a file. Does not include shortcuts.

---

### <a name="controls-tab"></a>Controls Tab

To assign a button or stick direction:

1. Click the name of the N64 input (e.g., "Start").  
2. Press the desired input before the countdown expires.  
3. To unbind, press **ESC** during countdown. (ESC cannot be assigned.)

- **Rapid Fire** — Slider adjusts toggle speed. Checkbox enables rapid fire for all buttons.  
- **Analog Stick Range** — Adjust if characters don’t respond correctly to full stick movement.  
- **Real N64 Range** — Emulates circular stick motion vs. Windows’ square calibration.  
- **Config 1 / Config 2** — Allows dual analog stick setups, switchable via modifiers.

---

<table align="center">
  <tr>
    <td><a href="config-nrage-controls">Controls</a></td>
    <td><a href="config-nrage-devices">Devices</a></td>
    <td><a href="config-nrage-mod">Modifiers</a></td>
    <td><a href="config-nrage-controller-pak">Controller Pak</a></td>
  </tr>
  <tr>
    <td><a href="config-nrage-trouble-rumble">Rumble Troubleshoot</a></td>
    <td><a href="config-nrage-faq">General FAQ</a></td>
    <td><a href="config-nrage-shortcuts">Shortcuts</a></td>
    <td>&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Controls Config Protocol Activated -->

