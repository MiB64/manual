---
title: Taking Screenshots
nav_order: 4
parent: Using MiB64
---

<style>
.zoom-pair {
  display: flex;
  gap: 12px;
  align-items: flex-start;
  position: relative;
}

.zoom-on-hover {
  display: inline-block;
  position: relative;
}

.zoom-on-hover img {
  display: block;
  cursor: zoom-in;
  transition: transform 0.3s ease;
  transform-origin: left center;
  position: relative;
  z-index: 1;
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
</style>

## <center>Taking Screenshots</center>
<b>
<div style="text-align: center;">
<div class="zoom-on-hover">
  <img src="/manual/asset/images/main.png" alt="MiB64 Main Browser" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

This section will take you through taking screenshots in MiB64.

- [Windows Printscreen](#windows)  
- [MiB64 Screenshot Function](#internal)  
- [Screenshot File Format](#format)  
- [Attribution](#credit)

<a name="windows"></a>
## <center>Windows Printscreen</center>
<b>

You can use the standard Windows screenshot functions:

- `PRTSCRN` — captures the entire desktop  
- `ALT+PRTSCRN` — captures the currently focused window

These keys copy the image to the clipboard. You must then paste it into an application like <i>Paint</i> or <i>Photoshop</i>. The clipboard typically holds only one image at a time, so taking another screenshot will overwrite the previous one. If MiB64 is windowed, `ALT+PRTSCRN` will include the GUI.

<a name="internal"></a>
## <center>MiB64 Screenshot Function</center>
<b>

MiB64 includes an internal screenshot function:

- Menu: `System > Screen Capture`  
- Shortcut: `F3`

This function writes sequentially numbered image files to your configured screenshots folder:

**Filename Format:**  
Game Internal Name 0000.jpg, Game Internal Name 0001.jpg ... Game Internal Name 9999.jpg

You can press the button as many times as you like (given enough storage space, up to 10,000 captures!) If you take shots in fullscreen, your shots will be of your native desktop resolution which depending on your settings can be very large. Screenshots taken while windowed will not include the MiB64 GUI.

<a name="format"></a>
## <center>Screenshot File Format</center>
<b>

Some video plugins (e.g. Icepir8's LLE) allow you to choose between PNG, BMP, and JPG formats via a dropdown. The internal MiB64 function writes files in the format currently selected. All screenshots will match the current video colour depth.

<a name="credit"></a>
## <center>Attribution</center>
<b>

All screenshots published from MiB64 or its video plugins should:

- Credit MiB64  
- Include a link to the [MiB64 website](https://www.mib64.net){:target="_blank" rel="noopener noreferrer"}  

---

<!-- Footer Navigation Block -->

<table align="center" style="width: 80%">
  <tr>
    <td style="text-align: center"><a href="using-mib64">Using MiB64</a></td>
    <td style="text-align: center"><a href="start-stop-reset-games">Start, Stop, Reset Games</a></td>
    <td style="text-align: center"><a href="save-load-games">Save & Load Games</a></td>
    <td style="text-align: center"><a href="/manual/manual/manual/cheats">Using Cheats</a></td>
  </tr>
  <tr>
    <td style="text-align: center"><a href="taking-screenshots">Taking Screenshots</a></td>
    <td style="text-align: center"><a href="multiple-instances">Multiple Instances</a></td>
    <td style="text-align: center"><a href="keyboard-shortcuts">Keyboard Shortcuts</a></td>
    <td style="text-align: center"><a href="using-mib64-troubleshooting-stability">Troubleshooting Stability</a></td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Screenshot Protocol Activated -->
