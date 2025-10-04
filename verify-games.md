---
title: Verifying Games
nav_order: 1
parent: Reference
---

## <center>Verifying Games</center>

Though hardly specific to MiB64, understanding and having good Games is so important to using MiB64 successfully that I'm going to cover it briefly here.

First you need to download the following from [Emutalk N64 Downloads](https://www.emutalk.net/forums/nintendo-64-downloads.158/){:target="_blank" rel="noopener noreferrer"}:

1. The latest version of ["GoodN64"](https://www.emutalk.net/threads/goodn64-2-02a.12068/){:target="_blank" rel="noopener noreferrer"} by Cowering  
2. ["GoodWindows"](https://www.emutalk.net/threads/goodwindows-2-4.12069/){:target="_blank" rel="noopener noreferrer"} by Master of Puppets  
   or ["GoodGUIv1.4"](https://www.emutalk.net/threads/goodgui-v0-97-goodguiv1-4.29155/){:target="_blank" rel="noopener noreferrer"} by polarz  
3. A file called ["bin.zip"](https://www.emutalk.net/threads/bin-zip.12070/){:target="_blank" rel="noopener noreferrer"} containing `zlib.dll` and other files you might need

If your Games are compressed, you need to download whatever utility is needed to decompress them—e.g., if they end in `.zip`, install WinZip; if `.rar`, install WinRAR, etc.

Have your unverified and decompressed Game files available somewhere on your hard drive, e.g. `C:\Temp`.

Unzip all the utilities listed above to one folder on your hard drive, e.g. `C:\Program Files\GoodTools\` (`zlib.dll` should end up in a `\bin` subfolder). Browse to the folder and run `GoodWindows.exe`.

1. Select mode "Good Tool"  
2. Select "Nintendo 64" as system. You will be prompted to browse to `GoodN64.exe`. Do so.  
3. Set "Directory to work on" to the folder containing your unverified Games (`C:\Temp` if following exactly)  
4. Keep "Options" set to "rename"  
5. Press the "Execute" button and wait until the program is finished. This may take some time.

Close GoodWindows and browse to your Game folder (`C:\Temp` if following exactly). You will find GoodWindows has created subfolders and text files. All known Games have been moved to a subfolder `N64ren`. Any Games not moved or renamed are *not known by GoodN64*—it's safe to assume they are bad and best to delete them.

So how do you know which Games are good? It's very simple: a good Game will now be in the `N64ren` subfolder and have `[!]` in its name. If it does not have `[!]` in the name, then something is wrong—the full key is included in GoodWindows under `Legend > Good Tools`.

Only `[!]` Games are supported by MiB64. If your Game is not good, find another. Usually bad Games don't even start, but sometimes they fail midway during a game—you do not want this!

---

<!-- Footer Navigation Block -->

<table align="center" style="width: 80%">
  <tr>
    <td style="text-align: center"><a href="reference">Reference</a></td>
    <td style="text-align: center"><a href="verify-games">Verifying Games</a></td>
    <td style="text-align: center"><a href="known-issues">Known Issues</a></td>
    <td style="text-align: center"><a href="language-files">GUI Translation</a></td>
  </tr>
  <tr>
    <td style="text-align: center"><a href="browser-data-sources">Browser Data Sources</a></td>
    <td style="text-align: center"><a href="min-specs">Minimum Specs</a></td>
    <td style="text-align: center"><a href="feature-lists">Feature Lists</a></td>
    <td style="text-align: center;">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Reference Protocol Activated -->
