---
title: Rumble Troubleshoot
nav_order: 5
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

## <center><b>N-Rage MiB64 Input Configuration — Troubleshooting Rumble</b></center>
<b>

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_Legacy_Input_Controller_Pak_3.png" alt="Controller Pak Tab" width="320" height="224" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

**Q: My device doesn't show up in the list.**  
**A1:** If you're using an X360 or other "XInput" controller, you need to download and configure the XBCD drivers. These provide DirectInput force feedback support as well as a slew of tweak options.  
[http://xbcd360guide.50webs.com/download.html](http://xbcd360guide.50webs.com/download.html)  
**A2:** First make sure you've plugged in the device before running your emulator. This updates the list of devices. Also, this list only shows DirectInput devices that support force feedback; you do not need to select a device here to assign buttons.  
**A3:** Have you assigned your device to another controller already? You can only assign rumble devices to one N64 controller, even if the other device's controller pak is set to "None". Check the Rumble Pak device in the other 3 controller tabs.

**Q: I can select my device, but Test Rumble doesn't work.**  
**A:** First, make sure you have the newest drivers for your controller; check the website of your controller's manufacturer. Also, some controllers have a switch or button that turns force feedback on and off (my Logitech gamepad is one of them), so you should check for that. As a last resort, try restarting the emulator and running the game anyway, and see if it works. For some reason, some controllers don't rumble in the config panel but rumble just fine in the game.

**Q: Test rumble works OK, but rumble in the game doesn't work.**  
**A:** Try the following:

- Are you certain that the game rumbles on the real N64? Try running a game like *Ocarina of Time*; the game should rumble after selecting a savegame.  
- Try restarting the emulator; sometimes clicking the Test Rumble button can cause rumble in-game to stop working, especially if you enter the configuration screen while emulation is running.  
- Many N64 games only support hot-plugging of rumble paks at certain times. If you're having this issue after using shortcuts or after restoring an emulator save state, try resetting the game with rumble pak selected.

If none of these fix the issue, post to the stickied thread in the Plugins category on emutalk.net with the name of the game you're running and the type of controller you're using.

<table align="center">
  <tr>
    <td style="text-align: center;"><a href="config-nrage-controls">Controls</a></td>
    <td style="text-align: center;"><a href="config-nrage-devices">Devices</a></td>
    <td style="text-align: center;"><a href="config-nrage-mod">Modifiers</a></td>
    <td style="text-align: center;"><a href="config-nrage-controller-pak">Controller Pak</a></td>
  </tr>
  <tr>
    <td style="text-align: center;"><a href="config-nrage-trouble-rumble">Rumble Troubleshoot</a></td>
    <td style="text-align: center;"><a href="config-nrage-faq">General FAQ</a></td>
    <td style="text-align: center;"><a href="config-nrage-shortcuts">Shortcuts</a></td>
    <td style="text-align: center;">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Rumble Troubleshoot Protocol Activated -->
