---
title: Feature Lists
nav_order: 6
parent: Reference
---

## <center>Feature Lists</center>

This page is intended for more advanced or curious users. If you meet the [Minimum Specs](min-specs-system), you already have everything covered and don’t need to worry about this!

MiB64 is compiled with Microsoft Visual Studio 19.

MiB64 uses the following extended CPU instruction sets if detected on your system:

- MMX  
- SSE  
- 3Dnow!  
- SSE2  
- SSSE3  
- SSE4.1  
- AVX  
- AVX2  
- LZCNT

These are mostly used in the video plugin and RSP. The emulator is tested to run without any of these instructions, but a minimum of SSE2 is recommended.

---

### TextureOpCaps (Jabo’s Direct3D Plugins)

Your hardware and drivers must support **all** of these features for good quality emulation. Usage varies by game:

- DISABLE  
- SELECTARG1  
- SELECTARG2  
- MODULATE  
- MODULATE2X  
- MODULATE4X  
- ADD  
- ADDSIGNED  
- ADDSIGNED2X  
- SUBTRACT  
- ADDSMOOTH  
- BLENDDIFFUSEALPHA  
- BLENDTEXTUREALPHA  
- BLENDFACTORALPHA  
- BLENDTEXTUREALPHAPM  
- BLENDCURRENTALPHA  
- MODULATEALPHA_ADDCOLOR  
- MODULATECOLOR_ADDALPHA  
- MODULATEINVALPHA_ADDCOLOR  
- MODULATEINVCOLOR_ADDALPHA

We no longer recommend the use of Jabo Plugins—they are outdated. Watch this space for updated Ice-related specs.

You can check your hardware’s support by downloading and running the Microsoft DirectX Caps Viewer. These features were not present in many systems at the time of release.

---

### Graphics Plugin Requirements

Most requirements are standard:

- Ability to do at least two textures per pass  
  (Multipass was removed in v1.2 due to fog rendering limitations)  
- Efficient texture memory usage (16MB graphics RAM suggested)  
- Internal geometry pipeline uses SSE and some 3Dnow!  
- Hardware clipping support is important for internal pipeline  
- Lighting is always done internally

---

### Framebuffer Performance

Primary framebuffer emulation depends heavily on memory copy speed. These operations are rarely used by games:

- Matrox cards are unusually fast (despite poor 3D features)  
- nVidia cards are relatively slow  
- A fast system is required for viable framebuffer use

---

### OpenGL Plugin Notes

The OpenGL plugin (not included in v1.4+) requires an nVidia TNT or higher card due to proprietary extensions not part of OGL 1.2/1.3 spec. It’s mostly experimental and rarely better than Direct3D—not due to API quality, but developer path.

---

### Input Plugin Notes

The default input plugin uses DirectInput and should work with most devices. However, it doesn’t support all DX controls.  
The N-Rage Legacy plugin supports more controls.

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
    <td style="text-align: center"><a href="min-specs-system">Minimum Specs</a></td>
    <td style="text-align: center"><a href="feature-lists-system">Feature Lists</a></td>
    <td style="text-align: center;">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Feature Lists Protocol Complete -->
