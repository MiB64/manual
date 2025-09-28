---
title: Feature Lists
nav_order: 2
parent: System Requirements
---

# Feature Lists

This page is intended for more advanced or curious users.  
If you meet the [system requirements](min-specs.md), then you already have everything covered and don't need to worry about this.

MiB64 is compiled with Microsoft Visual Studio 19.

MiB64 uses the following extended CPU instruction sets if they are detected on your system:

- MMX
- SSE
- 3Dnow!
- SSE2
- SSSE3
- SSE4.1
- AVX
- AVX2
- LZCNT

These are mostly used in the video plugin and RSP.  
The emulator is tested to run without any of these instructions, but a minimum of SSE2 is recommended.

---

## Jabo's Direct3D Plugin TextureOpCaps

Your hardware and drivers must support **all** of the following features for good quality emulation.  
Exactly which are used varies from game to game.

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
- MODULATEALPHA-ADDCOLOR
- MODULATECOLOR-ADDALPHA
- MODULATEINVALPHA-ADDCOLOR
- MODULATEINVCOLOR-ADDALPHA

We no longer recommend the use of Jabo Plugins as they are outdated.  
Watch this space for updated Ice-related specs.

You can see which features your hardware supports by downloading and running the Microsoft DirectX Caps Viewer.  
These features were not present in a large number of installed systems at the time of release.

---

## Graphics Plugin Requirements

Most requirements are already fairly standard, such as the ability to do at least two textures per pass.  
Multipass was removed in v1.2 because it's not possible to render fog properly with it.

- Texture memory usage is efficient; at least 16MB graphics RAM is suggested.
- The internal geometry pipeline makes extensive use of SSE and some use of 3Dnow!
- Hardware clipping support is important if using the internal pipeline.
- Lighting is always done internally regardless of pipeline.

---

## Framebuffer Performance

Primary framebuffer emulation performance depends on how fast your hardware handles memory copy operations.  
These are not commonly used by computer games.

- Matrox cards are unusually fast at this (despite poor 3D feature set).
- nVidia cards are relatively slow.
- A very fast system is required for framebuffer use to be viable.

---

## OpenGL Plugin Notes

The OpenGL plugin (not included in v1.4+) requires an nVidia TNT or higher card.  
It uses proprietary extensions not part of the OGL 1.2/1.3 spec.

This plugin is mostly experimental and rarely superior to Direct3D.  
This is due to development path, not inherent API differences.

---

## Input Plugin Notes

- Secondary video devices (e.g. 3dfx Voodoo1/2) are not supported.
- The default input plugin uses DirectInput and is generally flexible.
- N-Rage Legacy plugin supports more controls than the default.

---

## Navigation

- [Back to Requirements](requirements.md)
- [Next: Minimum Specs](min-specs.md)

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Feature Lists Protocol Complete -->
