---
title: Language Selection
nav_order: 8
parent: Settings (Application)
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

## <center>Configuration: Language</center>
<b>
<div style="text-align: center;">
  <p><strong>File > Language (No /Lang Folder present)</strong></p>
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/lang_1.png" alt="Language Dialog - No Lang Folder" width="300" height="260" />
  </div>
  <p><strong>Hover to zoom</strong></p>
  <p>On load if /Lang Folder is present in Root /Lang</p>
</div>

<!-- ClauseEcho: Interactive Image -->

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/lang_4.png" alt="Language Selection Prompt" width="300" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

The first time MiB64 is started, it asks you to choose a language if the Lang Folder is present.  
The choices available depend on the contents of the `/Lang` folder. MiB64 v1.0 shipped with a reasonable—but of course far from complete—set of translations included (thanks to everyone who made them!).

If the language you want is not in the list, [seek an updated/alternative file](updating-files) or [make/edit one yourself](language-files)!

---

<p style="text-align: center;"><strong>File > Language (/Lang Folder present)</strong></p>

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/lang_3.png" alt="Language Menu" width="300" height="260" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

To change languages at a later date, use the Language menu under the File menu in MiB64.  
Simply click an entry in the list and you should see the GUI text update immediately.

---

<table align="center">
  <tr>
    <td style="text-align: center;"><a href="app-settings">Settings</a></td>
    <td style="text-align: center;"><a href="app-plugins">Plugins</a></td>
    <td style="text-align: center;"><a href="app-directories">Directories</a></td>
    <td style="text-align: center;"><a href="app-options">Options</a></td>
    <td style="text-align: center;"><a href="app-game-selection">Game Selection</a></td>
  </tr>
  <tr>
    <td style="text-align: center;"><a href="app-advanced">Advanced</a></td>
    <td style="text-align: center;"><a href="app-game-settings">Game Settings</a></td>
    <td style="text-align: center;"><a href="app-game-information">Game Information</a></td>
    <td style="text-align: center;"><a href="app-language">Language Selection</a></td>
    <td style="text-align: center;">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: app-language.md Anchor Fidelity Restored -->
<!-- VaultEcho: Menu Structure List enforced. app-language.md locked at nav_order: 8 under Settings (Application). -->
