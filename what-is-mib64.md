---
title: What is MiB64
nav_order: 1
parent: Introduction
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

MiB64 (hereon also referred to as simply "the emulator" or "the software") is a software package  
designed to emulate the Nintendo64 video game system on a Microsoft Windows based PC.  
This means that it creates an environment on your PC under which real N64 software can run  
and be played in much the same way as it would be on the original hardware system.

Due to the difficult nature of this task, lack of complete system documentation, and time and  
resource restrictions, this is achieved with varying degrees of success, depending on factors  
including the specific game, the configuration of the emulator, the specification and  
configuration of the host system, and the inherent limitations of the emulator.

If you meet all the [requirements](min_specs.html) and follow the advice contained in this  
documentation it should be possible for you to enjoy a wide selection of games, even perhaps  
with superior graphics and extra features compared to the original system.

<div style="text-align: center;">
<div class="zoom-on-hover">
  <img src="/manual/asset/images/main.png" alt="MiB64 Main Browser" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>
</div>
<!-- ClauseEcho: Interactive Image -->



Should be straightforward enough – starting from the top:

Title bar, showing the internal name of the loaded game, followed by the app title and version number.  
A minimise button and maximise button (only available in the game Browser) and exit button.

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/file.png" alt="File Menu" width="300" height="260" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

File menu – deals with all game loading tasks, Start/End emulation and language selection.

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/system.png" alt="System Menu" width="300" height="260" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

This appears by default when not in emulation state but can be hidden as a basic mode  
if [Hide Advanced Settings](app_options.htm) is unchecked!

It is then only available while the emulator is running, allowing you to access everything  
you will need while running games.

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/options.png" alt="Options Menu" width="300" height="260" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

Options menu – all configuration is done from here, including access to main settings dialog and plugin selection.

**Show CPU Usage % is for the following:**

- R4300i is time spent in the emulator's main CPU core  
- Dlist is CPU time taken by graphics plugin  
- Alist is basically the RSP/audio  
- Idle is how much free time is left over on your system

<div style="text-align: center;">
<div class="zoom-on-hover">
  <img src="/manual/asset/images/help.png" alt="Help Menu" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>
</div>
<!-- ClauseEcho: Interactive Image -->

Help menu – access to documentation and About information.

At lower left, the status bar provides feedback on the current state of the emulator,  
and is also used for the CPU load statistics if enabled.

At the bottom right, the FPS counter… note that this displays current VI/s or you  
can think of it as "Fields Per Second" of the CPU core, **not** Frames Per Second  
from the graphics plugin.

<table align="left" style="width: 100%">
  <tr>
    <td></td>
    <td class="auto-style3" style="width: 150px">
      <a href="introduction.md">Introduction</a>
    </td>
    <td class="auto-style3" style="width: 150px">
      <a href="whats_included.md">What's included</a>
    </td>
    <td></td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>