---
title: Language Selection
nav_order: 9
parent: Application Settings
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

# Configuration: Language

Options → File → Language

---

## <a name="Lang_Folder_Absent"></a>When No `/Lang` Folder Is Present

<div class="zoom-on-hover">
  <img src="/manual/asset/images//lang_1.png" alt="No Lang Folder Present" style="width:220px;" />
</div>
<p><strong>Hover to zoom</strong></p>

If no `/Lang` folder is present in the root directory, MiB64 will not prompt for language selection on first launch.

---

## <a name="Lang_Folder_Present"></a>When `/Lang` Folder Is Present

<div class="zoom-on-hover">
  <img src="/manual/asset/images//lang_4.png" alt="Lang Folder Present" style="width:220px;" />
</div>
<p><strong>Hover to zoom</strong></p>

On first launch, MiB64 will prompt you to choose a language if the `/Lang` folder is present.  
Available choices depend on the contents of that folder.

MiB64 v1.0 shipped with a reasonable—but incomplete—set of translations.  
If your preferred language is missing:

- [Seek updated or alternative files](updating_files.md)
- [Create or edit your own language file](language_files.md)

---

## <a name="Change_Language_Later"></a>Changing Language Later

File → Language (when `/Lang` folder is present)

<div class="zoom-on-hover">
  <img src="/manual/asset/images//lang_3.png" alt="Language Menu" style="width:220px;" />
</div>
<p><strong>Hover to zoom</strong></p>

To change languages later, use the Language menu under File.  
Click an entry in the list and the GUI text will update immediately.

---

## Navigation Footer

```markdown
- [Settings](app_settings.md)
- [Plugins](app_plugins.md)
- [Directories](app_directories.md)
- [Options](app_options.md)
- [Game Selection](app_game_selection.md)
- [Advanced](app_advanced.md)
- [Game Settings](app_game_settings.md)
- [Game Notes](app_game_notes.md)
- [Shell Integration](app_shell_integration.md)
- [Language Selection](app_language.md)

<!-- ClauseEcho: Language Selection Protocol Complete -->