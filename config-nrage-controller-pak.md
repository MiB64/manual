---
title: Controller Pak Config
nav_order: 4
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

## <center><b>N-Rage MiB64 Input Configuration — Controller Pak Tab</b></center>
<b>

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_MiB64_Input_Controller_Pak_1.png" alt="Controller Pak Tab" width="320" height="224" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

One of the coolest features on the original N64 was the addition of modules that plugged into a port on the bottom of each controller. NRage DirectInput natively supports Memory Paks, the Rumble Pak, and the Transfer Pak; it also should support any pak through a real N64 controller hooked up to your computer through an Adaptoid. You can select the type of controller pak you want the emulator to see as plugged in to your controller.

There is one setting common to all controller paks, and that is the **RawMode** checkbox. If this is checked, it means that the NRage plugin will handle all controller pak data. If it is not checked, it means that your N64 emulator is responsible for handling all controller pak data. Most people will want to leave this checked. It is also probably a very bad idea to toggle this while a game is running, so if you do want to change it, use a save state, stop emulation, and then change it.

If RawMode is unchecked, you won't be able to set anything here besides the pak type. If it's checked, you'll see some options for the pak type you've selected (if you've selected one).

**None** means that no pak will be plugged in. The N64 will see that there is no peripheral connected to the controller.

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_MiB64_Input_Controller_Pak_1.png" alt="Controller Pak Tab" width="320" height="224" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

**Mem Pak** lets you choose a memory pak directory, choose a mempak (by clicking on it in the list), create new mempaks in the selected directory, and delete mempaks. If you select a mempak in the box on the left, the box on the right will show what savegames are present on that pak, as well as how many blocks each one uses (out of a maximum 123 blocks) and the region of the game that saved it. In the example above, I've selected a mempak with Japanese savegames; as you can see, the names still show up properly.  
**Format MemPak** *will completely erase the mempak*, so be careful. The other three buttons allow you to export and import "notes" in a64 format, and also delete them. A "note" is like a game save file on a mempak; each mempak can have at most 16 notes. Be aware that a few games have certain expectations about their savegames being stored in a certain order or in a set. Messing around with individual notes shouldn't cause problems in most cases, but has the potential to crash games and at worst delete your savegames; to be safe, make a backup of your mempak file before you try to modify it.

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_MiB64_Input_Controller_Pak_3.png" alt="Controller Pak Tab" width="320" height="224" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

**Rumble Pak** lets you set options for force feedback, if you have a device that supports it. The drop-down list will show any detected force feedback devices compatible with DirectInput. As you can see from the picture, if you haven't selected a compatible device then only **Visual Rumble** can be toggled. After selecting a device, the relevant options will become available.  
**Constant Force** uses one fixed value for the rumble strength, while **Ramp Force** starts with a fixed value and quickly drops off. "Constant Force" is closer to the original N64 controller, but some people like the feel of "Ramp Force" better.  
**Direct Rumble** will only be enabled if you have an Adaptoid plugged in, and sends rumble commands directly to the Adaptoid driver; if you're using a real N64 controller, you should use this or set the pak type to **Adaptoid**.  
The **Visual Rumble** tickbox flashes the LEDs on your keyboard if possible when a rumble command is sent by the N64.  
**Rumble Strength** sets the relative strength of the controller rumble, and **Test Rumble** tries to send a rumble command to make sure your controller is set up properly. DirectInput force feedback can be a bit quirky, so if you have trouble please see the separate troubleshooting section.

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_MiB64_Input_Controller_Pak_4.png" alt="Controller Pak Tab" width="320" height="224" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

**Transfer Pak** lets you choose Gameboy files for transfer pak emulation. The transfer pak is used to allow you to load character data or enable special features in certain N64 games. Select matching ROM (Gameboy cart) and RAM (savedata) files. For some games, like *Perfect Dark*, you only need the ROM, but for games that read character data you will need both, because the N64 game reads from the ROM header to figure out what game pak you have plugged in. You will need to use a separate Gameboy emulator to play the Gameboy games (and they should create the RAM files when they first run.) Transfer pak emulation works quite well, but as with memory pak files you should always keep backups, just in case.

**Adaptoid Pak** will only appear if you have an Adaptoid plugged in when the configuration screen is opened. It lets you use your real N64 controller with real native paks. Why wouldn't you just use the Adaptoid plugin built into your emulator? Well, because with NRage you can use an Adaptoid on controller 1, a PC gamepad on controller 2, and a keyboard and mouse on controller 3.

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

<!-- ClauseEcho: Controller Pak Config Protocol Activated -->
