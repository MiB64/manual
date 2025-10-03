---
title: Feature Lists
nav_order: 2
parent: System Requirements
---

## <center>Feature Lists</center>

This page is intended for more advanced or curious users only.  
If you meet the [minimum specs](min-specs), you already have everything covered and don’t need to worry about this!

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

These are mostly used in the video plugin and RSP.  
The emulator is tested to run without any of these instructions, but a minimum of SSE2 is recommended.

---

Jabo’s Direct3D plugins use the following **TextureOpCaps**.  
Your hardware and drivers must support **all** of these features for good quality emulation.  
Which ones are used varies from game to game:

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

We no longer recommend the use of Jabo Plugins—they are outdated.  
Watch this space for updated Ice-related specs.

You can check your hardware support by downloading and running the **Microsoft DirectX Caps Viewer**.  
These features were not present in many systems at the time of release.

---

Most other graphics plugin requirements are fairly standard, such as:

- Ability to do at least two textures per pass  
  (Multipass was removed in v1.2 due to fog rendering issues)  
- Efficient texture memory usage (16MB graphics RAM suggested)  
- Internal geometry pipeline uses SSE and some 3Dnow!  
- Hardware clipping support is important if using the internal pipeline  
- Lighting is always done internally

---

**Framebuffer Emulation Performance**  
This depends heavily on your system’s memory copy speed.  
Matrox cards were unusually fast (despite poor 3D features), while nVidia was relatively slow at the time.  
A very fast system is required for viable framebuffer emulation.

---

**OpenGL Plugin Notes**  
(Not included in v1.4+)  
Requires an nVidia TNT or higher card due to proprietary extensions.  
This plugin is experimental and rarely superior to Direct3D.  
This is due to development path—not API superiority.

---

**Unsupported Devices**  
Secondary video devices (e.g. 3dfx Voodoo1/2) are not supported.

**Input Plugin Notes**  
The default input plugin uses DirectInput and is generally flexible.  
However, it doesn’t support all DX controls.  
The **N-Rage Legacy plugin** supports more control types.

---

<table align="left" style="width: 100%">
  <tr>
    <td></td>
    <td class="auto-style3" style="width: 145px">
      <a href="requirements">Requirements</a>
    </td>
    <td class="auto-style3" style="width: 136px">
      <a href="feature-lists">Feature Lists</a>
    </td>
    <td class="auto-style3" style="width: 145px">
      <a href="min-specs">Minimum Specs</a>
    </td>
    <td></td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Feature Lists Protocol Complete -->
