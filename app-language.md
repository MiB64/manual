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
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/lang_1.png" alt="Language Dialog (No Lang Folder)" style="width: 220px;" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

File → Language (No `/Lang` folder present)

---

On load, if `/Lang` folder is present in the root directory:

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/lang_4.png" alt="Language Prompt on First Launch" style="width: 220px;" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

The first time MiB64 is started, it asks you to choose a language if the `/Lang` folder is present. The choices available depend on the contents of that folder.

MiB64 v1.0 shipped with a reasonable—but incomplete—set of translations (thanks to all contributors!). If your desired language is missing, you can [seek an updated file](updating-files) or [create/edit one yourself](language-files).

---

File → Language (Lang folder present)

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/lang_3.png" alt="Language Selection Menu" style="width: 220px;" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

To change languages later, use the Language menu under the File menu in MiB64. Click an entry in the list and the GUI text will update immediately.

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

<!-- ClauseEcho: Language Selection Node Complete -->
