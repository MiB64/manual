---
title: General FAQ
nav_order: 6
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

## <center><b>N-Rage MiB64 Input Configuration — General FAQ</b></center>
<b>

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_MiB64_Input_Controls.png" alt="Controls Tab" width="320" height="224" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

**Q: I opened up the configuration panel and some of the buttons I had assigned to my controller are listed as "Unassigned." Help!**  
**A:** This will happen if the controller or gamepad in question isn't plugged in when you open the configuration screen. In this case, the plugin can't bind the keys properly (because your controller isn't plugged in), so it just leaves them unbound.  
However, it's usually not a big problem; just click Cancel, plug in your controller, and restart the emulator.  
If you click Save, this "Unassigned" status will become permanent. In that case, you'll have to rebind the controls.

**Q: I can't get modifiers to "stick".**  
**A:** Before you click Save or change tabs or create a new modifier, you MUST click the button marked "Apply Changes". Otherwise, your changes will be lost.

**Q: Every time I change my settings in the configuration panel, the settings stay for awhile and then get reset when I change ROMs/restore a save state. What's wrong?**  
**A:** Click "Save" instead of "Use".

**Q: In Pokémon Stadium games, I can't run games in the "Gameboy Tower".**  
**A:** This is mostly a limitation of current emulators. In the original games, the "Tower" let you play certain Gameboy carts emulated on the N64.  
Since an emulator within an emulator just compounds problems, you should use a separate Gameboy emulator to run your games instead.  
It would not be wise to run the N64 emulator and your Gameboy emulator at the same time, as if they both decide to write to RAM at the same time, your data could become corrupted.

**Q: When are you going to add Voice Pak support?**  
**A:** When are you going to send me a Voice Pak and an Adaptoid to play around with?  
In all seriousness, since only one game ever supported this accessory (*Hey You Pikachu!*) it is unlikely that I'll ever get around to adding support for it.  
Also, since the device is rather rare, the detection code for the pak hasn't even been written.  
But if you have a Voice Pak and an Adaptoid, it should work. In fact, if you have this setup, please post on the emutalk.net thread, and maybe I can get started on it. You know, for posterity's sake.

**Q: How can I make a language pack?**  
**A:** If you're a native speaker of a language other than English, and your language pack hasn't already been created, download the "NRage Language SDK" from this address:  
[NRage_DInput8_Lang_SDK.zip (WayBack Machine Link)](https://web.archive.org/web/20160405210449/http://www.randomwisdom.com/files/NRage_DInput8_Lang_SDK.zip)  Right click on the link and Save As.

Then follow the instructions in the included text file.

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

<!-- ClauseEcho: General FAQ Protocol Activated -->
