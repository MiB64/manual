---
title: GUI Translation
nav_order: 3
parent: Reference
---

## <center>Translation & Language Files</center>

**Background – how MiB64 finds translations**

When MiB64 is started it looks for all files ending `.pj.Lang` in the `\Lang\` subfolder, opens each file, takes the line beginning `#1 #` (which will be the internal name of the language) and uses all of these to populate the Language selection menu. Note that the filename itself is not used except by us to identify the files.

**Starting a new translation**

To make a new translation file for MiB64, simply copy one of the existing `.pj.Lang` files—it doesn't matter which, you'd probably take the original English—then open the copy in a text editor (such as Microsoft Notepad, included with Windows) and you can begin editing the text.

**Preserving file layout**

Be careful that you don't change the formatting (layout) of the file at all. Every line must start hash-number-hash (e.g. `#460#`), then open quotes (`"`), then the actual text you want, then close quotes (`"`). Anything prefixed by `//` or contained within `/* ... */` is a comment and will be ignored by the emulator—i.e. it is only for humans reading the file. Make sure you use Notepad to edit the file, not Word or some other complex program which might mess up the formatting.

**Line breaks**

Line breaks (the movement from one line to the next, or line spaces) are taken literally, so to start a new line of text—e.g. in an error message—you actually press ENTER in the translation file. Do not use the end quote (`"`) until the end of the last line. (Also, don't use quotes anywhere in your text!)

**Shortcuts**

To create keyboard shortcut keys, put a `&` symbol before the letter you want to use as a shortcut. For example, `#127# "&Load State"` in the `.Lang` file will become "**L**oad State" in the application, and pressing "L" when in the System menu will instantly load a state. These shortcut keys are optional. You cannot change the CTRL+ or Function key shortcuts via the language file.

Don't forget to test your file! Make sure it loads properly (if not, check for missing closing quotes), and that the text fits the space available (if not, abbreviate!).

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
