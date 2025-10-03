---
title: Settings (Application)
nav_order: 5
has_children: true
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
  position: relative;
  z-index: 1;
  transform-origin: left center;
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

/* Final fix for standalone zoomable images */
.zoom-single {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: max-content;
  text-align: center;
}

.zoom-single:hover img {
  transform: scale(1.5);
  transform-origin: center center;
  z-index: 999;
}
</style>

## <center>Settings (Application)</center>

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/config_settings.png" alt="Advanced Tab" width="300" height="214" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

Options → Settings

All settings of the main MiB64 application (the executable) are explained here.

Before you go any further, please read the [Beginners](beginners) section.  
After you have, please select a topic:

<table align="center">
  <tr>
    <td style="text-align: center;">
      <a href="app_settings">Settings</a>
    </td>
    <td style="text-align: center;">
      <a href="app_plugins">Plugins</a>
    </td>
    <td style="text-align: center;">
      <a href="app_directories">Directories</a>
    </td>
    <td style="text-align: center;">
      <a href="app_options">Options</a>
    </td>
  </tr>
  <tr>
    <td style="text-align: center;">
      <a href="app_game_selection">Game Selection</a>
    </td>
    <td style="text-align: center;">
      <a href="app_advanced">Advanced</a>
    </td>
    <td style="text-align: center;">
      <a href="app_game_settings">Game Settings</a>
    </td>
    <td style="text-align: center;">
      <a href="app_game_information">Game Information</a>
    </td>
  </tr>
  <tr>
    <td style="text-align: center;">
      <a href="app_language">Language Selection</a>
    </td>
    <td style="text-align: center;">&nbsp;</td>
    <td style="text-align: center;">&nbsp;</td>
    <td style="text-align: center;">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Application Settings Protocol Activated -->
