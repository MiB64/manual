---
title: What is MiB64
nav_order: 1
parent: Introduction
---

<style>
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
  transform-origin: center center;
}
.zoom-on-hover:hover img {
  transform: scale(1.5);
  z-index: 999;
}
</style>

## What is MiB64?

MiB64 (hereon also referred to as simply "the emulator" or "the software") is a software package designed to emulate the Nintendo 64 video game system on a Microsoft Windows-based PC. It creates an environment on your PC under which real N64 software can run and be played in much the same way as it would on the original hardware system.

Due to the difficult nature of this task, lack of complete system documentation, and time and resource restrictions, this is achieved with varying degrees of success depending on factors including the specific game, the configuration of the emulator, the specification and configuration of the host system, and the inherent limitations of the emulator.

If you meet all the [requirements](min_specs.html) and follow the advice contained in this documentation, it should be possible for you to enjoy a wide selection of games—even with superior graphics and extra features compared to the original system.

<div class="zoom-on-hover">
  <img src="/manual/asset/images/main.png" alt="MiB64 Main Browser" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>

<!-- ClauseEcho: Interactive Image -->

---

### Interface Overview

**Title Bar**  
Displays the internal name of the loaded ROM, followed by the app title and version number. Includes minimize, maximize (ROM Browser only), and exit buttons.

<div class="zoom-on-hover">
  <img src="/manual/asset/images/file.png" alt="File Menu" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>

<!-- ClauseEcho: Interactive Image -->

**File Menu**  
Handles ROM loading, Start/End emulation, and language selection.

<div class="zoom-on-hover">
  <img src="/manual/asset/images/system.png" alt="System Menu" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>

<!-- ClauseEcho: Interactive Image -->

**System Menu**  
Appears by default when not in emulation state. Can be hidden as a basic mode if [Hide Advanced Settings](app_options.htm) is unchecked. Only available while the emulator is running.

<div class="zoom-on-hover">
  <img src="/manual/asset/images/options.png" alt="Options Menu" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>

<!-- ClauseEcho: Interactive Image -->

**Options Menu**  
All configuration is done here, including access to the main settings dialog and plugin selection.

**Show CPU Usage %**  
- **R4300i**: Time spent in the emulator's main CPU core  
- **Dlist**: CPU time taken by graphics plugin  
- **Alist**: RSP/audio  
- **Idle**: Remaining free time on your system

<div class="zoom-on-hover">
  <img src="/manual/asset/images/help.png" alt="Help Menu" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>

<!-- ClauseEcho: Interactive Image -->

**Help Menu**  
Access to documentation and About information.

---

### Status Indicators

- **Status Bar** (lower left): Feedback on emulator state and CPU load stats  
- **FPS Counter** (bottom right): Displays VI/s (Fields Per Second) of the CPU core—not FPS from the graphics plugin

---

### Navigation

- [Introduction](introduction.html)  
- [What's included](whats_included.html)

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: What is MiB64 Protocol Complete -->
