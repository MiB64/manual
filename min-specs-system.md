---
title: Minimum Specs
nav_order: 5
parent: Reference
---

## <center>MiB64 Minimum System Specification</center>

This specification will be sufficient for you to enjoy *most* compatible games with good graphics, sound and control, subject to correct configuration and some limitations of the emulator. You are likely to suffer some performance problems, and you will not be able to use all the options in the emulator.

- **Operating system** (No support for Windows Vista and below)  
  - Microsoft Windows 7 and up

- **CPU**  
  - Intel or AMD processor with at least SSE2 support

- **RAM**  
  - 512MB or more

- **Graphics card**  
  - DirectX 8 capable (Icepir8s-MiB64-LLE)  
  - OpenGL 3.3 capable (Icepir8s-MiB64-LLE)

The plugins contain SSE optimisations; early Athlons did not have SSE.

The video device must be a primary device, have at least 16MB local memory and two texture units. Depending on the features supported by your video card, some content may not be displayed correctly and thus some games marked as compatible may suffer glitches or not be playable on your system. The exact features required vary from game to game.

*nVidia GeForce256* and *ATI Radeon* (early models) are suggested as realistic minimum video hardware. In conjunction with good quality drivers they have the required features. Newer cards mainly allow better resolutions, filtering, anti-aliasing and so on.

The following chipsets (thus any and all graphics cards based on them) can be considered **below minimum specification**:

- 3dfx Voodoo 1,2,3 (1,2 – not at all, 3 – poor image quality)  
- ATI Rage128, Rage Pro (poor image quality)  
- Intel i740, i810 (poor image quality)  
- Matrox G200, G400, G450 (poor image quality)  
- nVidia Riva128 (poor image quality)  
- S3 Savage 4, Savage 2000 (particularly bad, these cards hang)

An [explanation](feature_lists.html) of why these cards are not capable of producing good quality images in MiB64.

You may find that MiB64 is usable on a lower-specification system than described here, particularly with some games and careful configuration. If so, then enjoy—but please don't expect too much.

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

<!-- ClauseEcho: Minimum Specs Protocol Activated -->
