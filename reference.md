---
title: Reference
nav_order: 13
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

## <center>MiB64 Reference</center>

<b>
<div style="text-align: center;">
<div class="zoom-on-hover">
  <img src="/manual/asset/images/main.png" alt="MiB64 Main Browser" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

This section documents several aspects of the emulator that are not covered elsewhere. This information will probably only be of interest to more advanced users and people wanting to understand better how the system works. This is not a programmers' reference – please refer to the authors' documentation for such information.

Please select a topic from the list.

---

<!-- Footer Navigation Block -->

<table align="center" style="width: 80%">
  <tr>
    <td style="text-align: center"><a href="reference">Reference</a></td>
    <td style="text-align: center"><a href="verify-games">Verifying Games</a></td>
    <td style="text-align: center"><a href="known-issues">Known Issues</a></td>
    <td style="text-align: center"><a href="language-files">GUI Translation</a></td>
  </tr>
  <tr>
    <td style="text-align: center"><a href="browser-data-sources">Browser Data Sources</a></td>
    <td style="text-align: center"><a href="min-specs">Minimum Specs</a></td>
    <td style="text-align: center"><a href="feature-lists">Feature Lists</a></td>
    <td style="text-align: center;">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Reference Protocol Activated -->
