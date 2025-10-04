---
title: Start, Stop, Reset Games
nav_order: 13
---

## <center><b>Start, Stop, Reset Games</b></center>
<b>
<div style="text-align: center;">
<div class="zoom-on-hover">
  <img src="/manual/asset/images/browser.png" alt="MiB64 Game Browser" width="380" />
</div>
<p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

<a name="starting-games"></a>
## <center><b>Starting Games</b></center>
<b>
<p>This section will take you through starting, stopping, changing & resetting games in MiB64.</p>

There are several ways to start a game in MiB64:

1. [The Game Browser](#game-browser)  
2. File > Open Game  
3. Recent Games menu

---

<a name="game-browser"></a>
## <center><b>The Game Browser</b></center>
<b>

This is the generally recommended method of starting games, for many reasons—[read about the Game Browser here](using-mib64#game-browser).

---

<a name="file-open"></a>
## <center><b>File > Open Game</b></center>
<b>

It is possible to use a standard Windows file open dialogue to start games.  
Go File > Open Game, browse to your game file and double click the file—with the default settings the game will load and emulation will start automatically.

If you are using this method, you won't have the feedback provided by the Browser, so you should be sure that you are opening a supported game and be aware of possible issues etc.

---

<a name="recent-games"></a>
## <center><b>Recent Games Menu</b></center>
<b>

Most users will have a small number of games that they play regularly.  
To make it easy for you to access these games without wading through all your games, MiB64 saves a list of the most recently opened games in the File menu, under “Recent Games.”

Every time a game is started (unless it's already the most recent), it's added to the top of the list, and the others are all pushed down one place.

By default the list shows only the 4 most recently started games, but this is [adjustable](app-game-selection#max-remembered-games).

---

<a name="recent-directories"></a>
## <center><b>Recent Directories Menu</b></center>
<b>

Most users will have a small number of directories that they use regularly.  
To make it easy for you to access these games without wading through all your folders, MiB64 saves a list of the most recently used directories in the File menu, under “Recent Games.”

Every time a game directory is added (unless it's already the most recent), it's added to the top of the list, and the others are all pushed down one place.

By default the list shows only the 4 most recently added game directories, but this is [adjustable](app-game-selection#max-remembered-dirs).

---

<a name="stopping-games"></a>
## <center><b>Stopping & Changing Games</b></center>
<b>

If you are finished playing and want to leave MiB64 you can simply close the emulator like any normal Windows application (use the X, or File > Exit—see [shortcut](keyboard-shortcuts)).

There is no need to End Emulation before you quit.  
If you are going to be away for a short period of time you could leave the emulator paused (by [default](app-options), losing window focus or minimizing the window will automatically pause for you).

MiB64 does not prompt you to save and does not save automatically on exit, so do not forget to make a [state save](save-load-games) if you want to be able to pick up exactly where you left off.

You'll probably want to make a named save, so go System > Save As ([shortcut](keyboard-shortcuts)) to open the dialogue and type in a path and name you'll remember.

If you want to play a different game, you can go back to the Game Browser to make your selection by choosing File > End Emulation, or you can go ahead and load it directly from File > Open or the Recent Game menu, even while the old game is running.

MiB64 will automatically End Emulation of the old game and load and start the new one (without any prompts—be careful!).

---

<a name="resetting-games"></a>
## <center><b>Resetting Games</b></center>
<b>

In case you are not familiar with the N64 console, it has a reset button.  
Pressing this is equivalent to turning the power off and back on—it's just smoother and quicker.

Of course there is no direct power button equivalent on MiB64, but the reset is emulated—go System > Reset.  
Keyboard shortcut: **F1**

### Points to note:
1. There is no prompt to reset, so be careful—it happens instantly. Make sure you save your game if you want to, there is no way to go back (undo).  
2. On reset, MiB64 checks all core settings, so if you have made any changes to the RDS or general options they will take effect now.  
3. After resetting, MiB64 has no memory of any state loads before the reset.  
   In other words, the RDRAM (the game's memory space) is totally wiped clean.  
   This is significant if you are using hacks/cheat codes or have core errors—do a native save, reset the game, and load through the game menus.  
   This is a smart dodge that can save you when your states go bad or a combination of cheat codes ruins your game.

---

<!-- Footer Navigation Block -->

<table align="center" style="width: 80%">
  <tr>
    <td style="text-align: center"><a href="using-mib64">Using MiB64</a></td>
    <td style="text-align: center"><a href="start-stop-reset-games">Start, Stop, Reset Games</a></td>
    <td style="text-align: center"><a href="save-load-games">Save &amp; Load Games</a></td>
    <td style="text-align: center"><a href="/manual/manual/manual/cheats.html">Using Cheats</a></td>
  </tr>
  <tr>
    <td style="text-align: center"><a href="taking-screenshots">Taking Screenshots</a></td>
    <td style="text-align: center"><a href="multiple-instances">Multiple Instances</a></td>
    <td style="text-align: center"><a href="keyboard-shortcuts">Keyboard Shortcuts</a></td>
    <td style="text-align: center"><a href="using-mib64-troubleshooting-stability">Troubleshooting Stability</a></td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Start / Stop / Reset Protocol Activated -->
