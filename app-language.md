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

## <a name="Lang-Folder-Absent"></a>When No `/Lang` Folder Is Present

<div class="zoom-on-hover">
  <img src="/manual/assets/images/lang-1.png" alt="No Lang Folder Present" style="width:220px;" />
</div>
<p><strong>Hover to zoom</strong></p>

If no `/Lang` folder is present in the root directory, MiB64 will not prompt for language selection on first launch.

---

## <a name="Lang-Folder-Present"></a>When `/Lang` Folder Is Present

<div class="zoom-on-hover">
  <img src="/manual/assets/images/lang-4.png" alt="Lang Folder Present" style="width:220px;" />
</div>
<p><strong>Hover to zoom</strong></p>

On first launch, MiB64 will prompt you to choose a language if the `/Lang` folder is present.  
Available choices depend on the contents of that folder.

MiB64 v1.0 shipped with a reasonable—but incomplete—set of translations.  
If your preferred language is missing:

- [Seek updated or alternative files](updating-files.md)
- [Create or edit your own language file](language-files.md)

---

## <a name="Change-Language-Later"></a>Changing Language Later

File → Language (when `/Lang` folder is present)

<div class="zoom-on-hover">
  <img src="/manual/assets/images/lang-3.png" alt="Language Menu" style="width:220px;" />
</div>
<p><strong>Hover to zoom</strong></p>

To change languages later, use the Language menu under File.  
Click an entry in the list and the GUI text will update immediately.

---

## Navigation Footer

```markdown
- [Settings](app-settings.md)
- [Plugins](app-plugins.md)
- [Directories](app-directories.md)
- [Options](app-options.md)
- [Game Selection](app-game-selection.md)
- [Advanced](app-advanced.md)
- [Game Settings](app-game-settings.md)
- [Game Notes](app-game-notes.md)
- [Shell Integration](app-shell-integration.md)
- [Language Selection](app-language.md)

<!-- ClauseEcho: Language Selection Protocol Complete -->