---
title: Save & Load Games
nav_order: 2
parent: Using MiB64
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

## <center>Save & Load Games</center>
<b>
<div style="text-align: center;">
<div class="zoom-on-hover">
  <img src="/manual/asset/images/main.png" alt="MiB64 Main Browser" width="300" height="260" />
</div>
<p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

This section will take you through saving & loading game progress in MiB64.

- [native saves](#native)  
- [state saves](#state)  
- [importing and exporting](#import)

## <center>Points</center>
<b>

1. It is highly recommended that you make regular native saves. Although state saves usually work OK, this is not guaranteed due to many things that can go wrong in the core and memory of the emulator. Native saves are more reliable (and smaller!) than state saves. By using both methods (rather than just state saves) you have a backup if anything goes wrong.  
2. For state saving to work the Games must be identical - that is, the Game that the game was saved from must match exactly the one that the state is loaded into. You may be able to share native saves between different versions of a game, but you cannot ever do this with state saves. MiB64 tags state files with Game header information and will check for and prompt you on violation of this rule.  
3. Native save files must not be Read Only, games need to be able to read/write at any time. For example if you back up your save files to a CDR, when you copy them back to your harddrive they may still be marked read-only - you must change the attributes with Windows Explorer. MiB64 does not do this automatically, in case you don't want your file to be updated for any reason.

<a name="native"></a>
## <center>Native Saves</center>
<b>

To understand the game data saving and loading of MiB64, you must also understand the N64's own saving and loading systems (if you aren't already familiar with them), because MiB64 emulates all those systems.

There are four types of save system used on the N64...

- EEPROM (a cartridge save type), which comes in two sizes:  
  - 4Kbit EEPROM  
  - 16Kbit EEPROM  
- SRAM (a cartridge save type)  
- FlashRAM (a cartridge save type)  
- MemPak (an optional hardware accessory for the N64, plugs into controller*)

...which we will call the "native" N64 save systems (to differentiate them from state saving, which is something entirely different, see below).

The cartridge save types use either non-volatile memory (EEPROM, FlashRAM) or a battery (SRAM) to keep a small amount of writeable memory intact inside the actual game cartridge, when the power to the console is off. Although it is on the same PCB, this save memory is physically separate from the game chips.
MiB64 does not write to the Game file or anything like that. You don't have to worry about the difference between EEPROM, SRAM and FlashRAM, because all three are handled the same from your point of view. You should be aware that MemPaks, unlike the other save types, can be handled by input plugins, which is logical if you consider the original system again.

1. Whenever an N64 game would save to or load from its game cartridge, MiB64 automatically updates a file called `{internal Game name}.{type}`** on your hard drive (you can [configure folders](app_directories.html) to choose the location). If this file does not exist, it is created as soon as the Game is first booted, and is the only file MiB64 will use for this game.  
2. Whenever the N64 game would save to a Controller Pack (MemPak), either MiB64 creates a file on your hard drive, or the input plugin manages the saving process, depending on the capabilities and configuration of the input plugin (see [plugin selection](app_plugins.html)).

The resulting save files will be compatible with both other N64 emulators and a real N64 system (if you possess the means to insert and extract them—see importing and exporting).

*Mempak is required by some games to save, is an optional extra in some games, is not used at all in some games. Any particular game can use any one cartridge save type, and/or the Controller Pak. This is normally handled transparently by the emulator.

** For example, you are playing the game Mario64. Mario 64 uses the EEPROM save type, and your Game has the internal name "SUPER MARIO 64". Therefore the save file automatically created and managed by MiB64 will be called "SUPER MARIO 64.eep" in your [configured folder](app_directories.html).

<a name="state"></a>
## <center>State Saves</center>
<b>

In addition to emulating the native save types, MiB64 is also capable of saving the entire state of *itself*—everything that it needs to know to recreate an exact point in time during the emulation of a particular game.

State saving can be broken down into two types:

- slot saves ("Quick Save")  
- named saves ("Save As...")

A game saved and loaded in this way does not "know" that it has been saved and loaded—it is as if the interruption never happened. This is clearly something quite different to what you can do on a real N64. This is called "state saving", the resulting file is a "state save" or "saved state", and will be relatively large compared to a native save file.

State save files will not be compatible with other N64 emulators unless they explicitly support the state save file format (At the time of writing this, no other emulator does). It is worth noting that a state save file will also save any errors that may have occurred and be present in the memory of the emulator, and for this reason, state saves are generally less reliable than native saves, especially over a long period of time playing.

To provide you with more flexibility in state saving, a number of "slots" are provided. A "slot" is simply a number, which is associated with a particular keyboard key so that you can select the file with a single button press. The advantage of slots is that you can switch between them quickly, the disadvantage is that you might have trouble remembering what you put in each slot! Every region and version of a game has its own independent set of 20 slots, so don't worry about one game overwriting another.

- Default Slot0: `"Game Name.qs0.zip"` with a shortcut of `0`  
- Slot1: `"Game Name.qs1.zip"` with a shortcut of `1`, all the way to  
- Slot9: `"Game Name.qs9.zip"` with a shortcut of `9`  
- Then the cycle begins over with Shift+number for:  
- Slot10: `"Game Name.qs10.zip"` with a shortcut of `Shift+0`, all the way to  
- Slot19: `"Game Name.qsj19.zip"` with a shortcut of `Shift+9`

Save As... just means you can choose a filename and location for your state save file. This is good when you finish a session and want to make a note of where you were in the game.

It is normal for the system to pause for a short while while generating, compressing and writing the save file. The quicker your system, the shorter the pause.

<a name="import"></a>
## <center>Importing and Exporting</center>
<b>

- ...to and from other emulators  
- ...to and from a real N64 system

MiB64 is compatible with the N64 saves (not necessarily state saves) from other N64 emulators and a real N64 system, but you may need to byteswap the files (use e.g. [Azimer's saveswapper utility](http://www.apollo64.com/files/saveswap.zip)) and you will definitely need to rename the files to what MiB64 expects.
See your existing save folder for the correct file name if you are not sure what the filename should be, save in the game anywhere a file will be created and you can use that name. The format is also explained under "native saves" above.

---

<!-- Footer Navigation Block -->

<table align="center" style="width: 80%">
  <tr>
    <td style="text-align: center"><a href="using-mib64">Using MiB64</a></td>
    <td style="text-align: center"><a href="start-stop-reset-games">Start, Stop, Reset Games</a></td>
    <td style="text-align: center"><a href="save-load-games">Save & Load Games</a></td>
    <td style="text-align: center"><a href="/manual/manual/manual/cheats">Using Cheats</a></td>
  </tr>
  <tr>
    <td style="text-align: center"><a href="taking-screenshots">Taking Screenshots</a></td>
    <td style="text-align: center"><a href="multiple-instances">Multiple Instances</a></td>
    <td style="text-align: center"><a href="keyboard-shortcuts">Keyboard Shortcuts</a></td>
    <td style="text-align: center"><a href="using-mib64-troubleshooting-stability">Troubleshooting Stability</a></td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Save & Load Protocol Activated -->
