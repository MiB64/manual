---
title: Shortcuts
nav_order: 7
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

## <center><b>N-Rage MiB64 Input Configuration — Shortcuts Tab</b></center>
<b>

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_MiB64_Input_Shortcuts.png" alt="Shortcuts Tab" width="320" height="224" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

To the right of the four controller tabs is a tab labelled **Shortcuts**. Shortcuts are generic buttons you can use for changing pak types on the fly, and for "locking" the mouse. The former are pretty self-explanatory; they change the paktype to the indicated type.  
For the buttons that "switch" between mempak and another type of pak, pressing the button while a mempak is plugged in will switch to that other pak; if any other pak is plugged in, the key will switch to the mempak.

Mouse locking is set whenever any control is assigned to the mouse; it ensures that when you're clicking madly in windowed mode you won't inadvertently click on any menus.  
However, to turn it off to select from the menus in your emulator you'll need to use it, defaulted to the TAB key.

Finally, there's a tickbox labelled **Show messages**. If it is on, a message box will overlay on top of the emulator window when a shortcut is used.  
It can cause graphical anomalies and crashes with some graphics plugins, so if this happens turn it off.

You can also save and load your shortcuts to files, as well as restore their defaults, just like controller configurations.

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

<!-- ClauseEcho: Shortcuts Config Protocol Activated -->
