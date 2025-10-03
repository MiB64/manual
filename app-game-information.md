---
title: Game Information
nav_order: 7
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

## <center>Configuration: Game Information</center>
<b>
<div style="text-align: center;">
  <div class="zoom-pair">
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
    </div>
    <div class="zoom-on-hover">
      <img src="/manual/asset/images/game_information.png" alt="Game Information Dialog" width="155" />
    </div>
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<p style="text-align: center;">This tab is only available if <a href="app-options">Hide Advanced Settings</a> is unchecked!</p>

<!-- ClauseEcho: Interactive Images -->

---

Options > Settings > Game Information

---

### Controls available:

1. [Game Status](#o1) (drop-down menu)  
2. [Players](#o2) (drop-down menu)  
3. [Force Feedback](#o3) (drop-down menu)  
4. [Core Note](#o4) (text box)  
5. [Plugin Note](#o5) (text box)  
6. [Game Language](#o6) (text box)  
7. [User Note](#o7) (text box)

---

### Points

- When you make changes here, you are actually editing the MiB64 Game Database Settings (the file `MiB64.rds`). You can also edit this file directly in a text editor – advanced users only!  
- If you get in a mess, the only way to go back to the supplied settings is to replace `MiB64.rdb` (from the original downloaded archive).  
- There is no "reset to defaults" button or similar.

---

## "Game Status" <a name="o1"></a>

This drop-down menu shows a list of all the status categories found in the RDS. You may choose any of these you find correct for a particular game. To add or edit categories, you must edit the RDS in a text editor.

---

## "Players" <a name="o2"></a>

This drop-down menu shows a list of the amount of players a game supports found in the RDI. You may choose any of these. To add or edit categories, you must edit the RDI in a text editor.

---

## "Force Feedback" <a name="o3"></a>

This drop-down menu shows a choice of Yes or No for if a game supports Force Feedback (Rumble).

---

## "Core Note" <a name="o4"></a>

This is simply a text field which edits the line `Core Note=` for the current game in the RDS.

---

## "Plugin Note" <a name="o5"></a>

This is simply a text field which edits the line `Plugin Note=` for the current game in the RDS.

---

## "Game Language" <a name="o6"></a>

This is simply a text field which edits the line `GameLanguage=` for the current game in the RDI. It is best to write and display them like: English, French, German etc.

---

## "User Note" <a name="o7"></a>

This is simply a text field which adds and displays a personal note (`User Note`) for the current game in the RDN. It is purely for you the user to make notes to display in the Game Browser if you choose to do so.

---

You must refresh the Game Browser for any changes to any of these fields to take effect.

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

<!-- ClauseEcho: app-game-information.md Anchor Fidelity Restored -->
