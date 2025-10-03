---
title: Input (Controller) Config
nav_order: 10
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

## <center>Configuration: N-Rage MiB64 Input Plugin</center>
<b>

<div style="text-align: center;">
  <div class="zoom-pair">
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/config_controller.png" alt="Config Controller Dialog" width="300" height="214" />
    </div>
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/NRage_MiB64_Input_Controls.png" alt="NRage Controls Dialog" width="300" height="214" />
    </div>
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Images -->

Options > Configure Controller Plugin

This page covers configuration of the N-Rage MiB64 Input plugin.

Because the input plugin has so many options, they have been divided by the plugin’s tabs in the config dialog.  

---

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

<!-- ClauseEcho: Config Input Protocol Activated -->


