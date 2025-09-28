---
title: What is MiB64?
nav_order: 1
parent: Introduction
---

<style>
.zoom-on-hover {
  display: inline-block;
  position: relative;
}
.zoom-on-hover img {
  width: 300px;
  transition: transform 0.3s ease;
  cursor: zoom-in;
  transform-origin: left center;
  display: block;
}
.zoom-on-hover:hover img {
  transform: scale(1.5);
  z-index: 10;
}
</style>

# What is MiB64?

MiB64 (hereon also referred to as simply "the emulator" or "the software") is a software package designed to emulate the Nintendo 64 video game system on a Microsoft Windows–based PC.  
This means that it creates an environment on your PC under which real N64 software can run and be played in much the same way as it would be on the original hardware system.

Due to the difficult nature of this task, lack of complete system documentation, and time and resource restrictions, this is achieved with varying degrees of success—depending on factors including:

- The specific game
- The configuration of the emulator
- The specification and configuration of the host system
- The inherent limitations of the emulator

If you meet all the [requirements](min_specs.md) and follow the advice contained in this documentation,  
it should be possible for you to enjoy a wide selection of games—perhaps even with superior graphics and extra features compared to the original system.

<div class="zoom-on-hover">
  <img src="/manual/asset/images/main.png" alt="MiB64 Main Browser" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>

---

## Interface Overview

Should be straightforward enough—starting from the top:

- **Title bar**: Shows the internal name of the loaded ROM, followed by the app title and version number. Includes minimise, maximise (ROM Browser only), and exit buttons.

<div class="zoom-on-hover">
  <img src="/manual/asset/images/file.png" alt="File Menu" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>

- **File menu**: Handles ROM loading, Start/End emulation, and language selection.

<div class="zoom-on-hover">
  <img src="/manual/asset/images/system.png" alt="System Menu" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>

This appears by default when not in emulation state, but can be hidden as a basic mode if [Hide Advanced Settings](app_options.md) is unchecked.  
It is then only available while the emulator is running, allowing access to everything needed during gameplay.

<div class="zoom-on-hover">
  <img src="/manual/asset/images/options.png" alt="Options Menu" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>

- **Options menu**: Central hub for configuration, including access to the main settings dialog and plugin selection.

### Show CPU Usage %

- **R4300i**: Time spent in the emulator's main CPU core  
- **Dlist**: CPU time taken by graphics plugin  
- **Alist**: RSP/audio processing  
- **Idle**: Remaining free time on your system

<div class="zoom-on-hover">
  <img src="/manual/asset/images/help.png" alt="Help Menu" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>

- **Help menu**: Access to documentation and About information

---

## Status Indicators

- **Status bar (lower left)**: Feedback on emulator state and CPU load statistics (if enabled)
- **FPS counter (bottom right)**: Displays current VI/s ("Fields Per Second" of the CPU core), not frames per second from the graphics plugin

---

## Navigation

- [Back to Introduction](introduction.md)
- [Next: What's Included](whats_included.md)

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: What is MiB64 Protocol Complete -->
