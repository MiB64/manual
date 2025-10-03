---
title: Game Selection
nav_order: 4
parent: Settings (Application)
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

## <center>Configuration: Game Selection</center>
<b>
<div style="text-align: center;">
  <div class="zoom-pair">
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
    </div>
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/game_selection.png" alt="Game Selection Dialog" width="155" />
    </div>
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Images -->

This tab is only available if [Hide Advanced Settings](app_options) is unchecked!

---

Options → Settings → [Game Selection](#Game_Selection)

---

### <a name="Game_Selection"></a>Game Selection Options

- <a name="Max_Remembered_Games">Max # of Games Remembered</a> (Max 10) - These are shown in File > Recent Games.  
- <a name="Max_Remembered_Dirs">Max # of Game Dirs Remembered</a> (Max 10) - These are shown in File > Recent Game Directories.  
- Enable/Disable the Browser completely by toggling the Use Game Browser checkbox  
- <a name="Enable_Recursion">Enable/Disable Directory Recursion</a> by toggling the Directory Recursion checkbox  
- Add or Remove fields from the Browser by selecting (click on) the field you want to add or remove and clicking the Add or Remove button.  
- Change the order of fields by clicking the field you want to move and clicking Up or Down. Top to bottom in the window represent Left to Right in the browser.

---

### Browser Customisations

The following customisations can be made from within the browser itself:

- Resize the browser window by dragging the window edges  
- Maximise/Restore the browser window with the maximise/restore button  
- Resize the width of any column by dragging the edge of the column header  
- Sort by any column by clicking inside the column header. You can sort in either direction by repeated clicking.

---

<table align="center">
  <tr>
    <td class="auto-style3"><a href="app_plugins">Plugins</a></td>
    <td class="auto-style3"><a href="app_directories">Directories</a></td>
    <td class="auto-style3"><a href="app_options">Options</a></td>
    <td class="auto-style3"><a href="app_game_selection">Game Selection</a></td>
    <td class="auto-style3"><a href="app_advanced">Advanced</a></td>
  </tr>
  <tr>
    <td class="auto-style3"><a href="app_game_settings">Game Settings</a></td>
    <td class="auto-style3"><a href="app_game_information">Game Information</a></td>
    <td class="auto-style3"><a href="app_language">Language Selection</a></td>
    <td class="auto-style3">&nbsp;</td>
    <td class="auto-style3">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Game Selection Node Complete -->
