---
title: Directories
nav_order: 3
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

# Configuration: Directories

<div class="zoom-pair">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images//config_settings.png" alt="Config Settings Dialog" width="300" height="207" />
  </div>
  <div class="zoom-on-hover">
    <img src="/manual/asset/images//directories.png" alt="Directories Dialog" width="155" />
  </div>
</div>
<p><strong>Hover to zoom</strong></p>

Options → Settings → Directories

---

**N.B.** It is purely a matter of personal preference how you set these folders,  
but you *must* have the Plugin folder set correctly for MiB64 to start up properly.  
If valid plugins aren’t found at the configured path when MiB64 starts, you cannot launch games.

This is by design—plugins are essential.  
You can still access Options to correct the paths.

---

## Folder Types

MiB64 allows you to set up to five different folders:

1. **Plugin Directory** — All plugins must be placed together in one folder  
   *(default: `\Plugin\` subfolder of MiB64 root)*

2. **Game Directory** — MiB64 remembers the last used folder,  
   but you can force it to always use a specific one

3. **N64 Native Saves Directory** — All native save types are placed here  
   *(default: `\Save\` subfolder of MiB64 root)*

4. **Quick Save States Folder** — If you use state slots, files go here  
   *(default: same as native saves folder)*

5. **Screenshots Directory** — Used by the video plugin for screenshots  
   *(default: `\Screenshots\` subfolder of MiB64 root)*

---

Each folder can use a default path or one you choose.

You can type a path directly or browse using the “...” button.  
Press OK to confirm the path.

Press OK again to save your changes.

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Directory Configuration Protocol Complete -->
