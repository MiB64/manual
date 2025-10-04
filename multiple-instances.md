---
title: Multiple Instances
nav_order: 5
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

## <center>Multiple Instances</center>
<b>
<div style="text-align: center;">
<div class="zoom-on-hover">
  <img src="/manual/asset/images/main.png" alt="MiB64 Main Browser" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

This section will take you through multiple instances of MiB64.

You can have more than one copy of MiB64 open and running at the same time!

The ability to have multiple instances can be a good thing, if you want to compare two windows side by side for example, or a bad thing, if you don't understand that there can be complications, or do it accidently! (i.e. if you start another instance without noticing you already have one running).

### <center>Points:</center>

1. Only one instance can have access to a particular save file at a time. So if you try to open the same game twice, you can expect the second instance to be denied access to the save data.
2. Plugins could act in unexpected ways, depending on how they are written, for example, an audio plugin may only give sound from the first instance, or an input plugin may only send keypresses to the instance that has focus. The default plugins should work with all instances.
3. Following on from the point above, this could also be complicated by your DirectX and hardware and driver capabilties, for example, the number of 3D rendering surfaces your graphics card can manage, or the number of audio streams your sound card can handle. These may or may not be issues on your system.
4. Because the application uses a centralised database, you cannot keep configurations seperate for multiple instances of the same version of MiB64. (This was partly an intended effect).
5. Clearly, running more than one instance of MiB64 increases the system requirements dramatically. Don't expect any instance to run as well as it would on its own, unless you pause the others (if you only have one instance actually running at a time, and have sufficient memory, you shouldn't notice performance problems).

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

<!-- ClauseEcho: Multiple Instance Protocol Activated -->
