---
title: Devices Config
nav_order: 2
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

## <center><b>N-Rage MiB64 Input Configuration — Devices Tab</b></center>
<b>

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_MiB64_Input_Devices.png" alt="Devices Tab" width="320" height="224" />
  </div>	
    <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

This tab lets you set some device-specific settings. You can leave it alone, or you can tweak things. Here's what each slider and button does.

**Mouse Sensitivity** — X and Y adjust how sensitive the mouse is in each direction.  
People who want a small movement of the mouse to translate to a large movement on screen should move these sliders to the right.  
People who want a less twitchy mouse should move them to the left.

The bubbles for **Deadpan**, **Buffered**, and **Absolute** take a bit of explanation. Each changes how the mouse inputs are translated to joystick inputs.

**Deadpan** — The joystick is set off-center as long as the mouse is in motion. As soon as you stop moving the mouse, the joystick immediately centers itself.  
**Buffered** — Similar to Deadpan, except that large mouse movements are "distributed" over several frames. It works quite well for first-person shooters, but tends to feel more "drifty" than a native PC game. This is the default.  
**Absolute** — An imaginary "center point" is chosen. Moving the mouse away from this point holds the joystick in that direction. If you're moving an onscreen cursor (like the aiming mode of *GoldenEye*) you want to use this mode.

**Keyboard Absolute** — X and Y are a different way of handling N64 analog stick inputs.  
Normally, the joystick is held in a direction as long as you press the keyboard key.  
Using Absolute Keyboard settings, the keys will control the absolute position of the joystick.  
This means if you hold the "right" key for a while, the virtual N64 joystick moves to the right.  
When you let go, it stays there. To move it back to the center, you have to press and hold the "left" key for a short time (but if you hold it too long, the joystick will be pressed left).

**Gamepad Deadzone** — Controls how far you can move a gamepad control before it registers as having moved.  
If you're using a high quality gamepad, you can theoretically move this to 0%.  
If your character is having spasms without you touching the controller, set this higher.  
Setting it too high sacrifices fine grain control, making it harder to sneak around in games that require you to press the joystick just a little bit.

<table align="center">
  <tr>
    <td style="text-align: center;"><a href="config_nrage_controls.html">Controls</a></td>
    <td style="text-align: center;"><a href="config_nrage_devices.html">Devices</a></td>
    <td style="text-align: center;"><a href="config_nrage_mod.html">Modifiers</a></td>
    <td style="text-align: center;"><a href="config_nrage_controller_pak.html">Controller Pak</a></td>
  </tr>
  <tr>
    <td style="text-align: center;"><a href="config_nrage_trouble_rumble.html">Rumble Troubleshoot</a></td>
    <td style="text-align: center;"><a href="config_nrage_faq.html">General FAQ</a></td>
    <td style="text-align: center;"><a href="config_nrage_shortcuts.html">Shortcuts</a></td>
    <td style="text-align: center;">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Devices Config Protocol Activated -->
