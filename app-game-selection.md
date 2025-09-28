---
title: Game Selection
nav_order: 5
parent: Application Settings
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

# Configuration: Game Selection

<div class="zoom-pair">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images//config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
  </div>
  <div class="zoom-on-hover">
    <img src="/manual/asset/images//game_selection.png" alt="Game Selection Dialog" width="155" />
  </div>
</div>
<p><strong>Hover to zoom</strong></p>

Options → Settings → <a name="Game_Selection">Game Selection</a>

---

**Note:** This tab is only available if [Hide Advanced Settings](app_options.md#o5) is unchecked.

---

## Game Browser Controls

- <a name="Max_Remembered_Games"></a>**Max # of Games Remembered** (Max 10)  
  Shown in `File > Recent Games`

- <a name="Max_Remembered_Dirs"></a>**Max # of Game Dirs Remembered** (Max 10)  
  Shown in `File > Recent Game Directories`

- **Enable/Disable Browser**  
  Toggle the “Use Game Browser” checkbox

- <a name="Enable_Recursion"></a>**Enable/Disable Directory Recursion**  
  Toggle the “Directory Recursion” checkbox

- **Add/Remove Fields**  
  Select a field and click Add or Remove

- **Reorder Fields**  
  Select a field and click Up or Down  
  *(Top to bottom = Left to right in browser)*

---

## Browser Window Customization

- Resize the browser window by dragging edges
- Maximize/Restore using the window button
- Resize column widths by dragging header edges
- Sort by any column by clicking its header  
  *(Click again to reverse sort direction)*

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Game Selection Protocol Complete -->
