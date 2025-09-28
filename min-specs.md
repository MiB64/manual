---
title: Minimum Specs
nav_order: 3
parent: System Requirements
---

# MiB64 Minimum System Specification

This specification will be sufficient for you to enjoy *most* compatible games with good graphics, sound, and control—subject to correct configuration and some limitations of the emulator.  
You may experience performance issues and will not be able to use all emulator options.

---

## Minimum Requirements

- **Operating System**  
  - Microsoft Windows 7 and up  
  - *(No support for Windows Vista and below)*

- **CPU**  
  - Intel or AMD processor with at least SSE2 support

- **RAM**  
  - 512MB or more

- **Graphics Card**  
  - DirectX 8 capable *(Icepir8s-MiB64-LLE)*  
  - OpenGL 3.3 capable *(Icepir8s-MiB64-LLE)*

> Note: Plugins contain SSE optimisations. Early Athlons did not support SSE.

---

## Graphics Considerations

- The video device must be a **primary device**
- Must have **at least 16MB local memory** and **two texture units**
- Depending on your card’s features, some games may suffer glitches or fail to run
- Required features vary by game

Suggested minimum video hardware:

- *nVidia GeForce256*
- *ATI Radeon* (early models)

These cards, with good drivers, meet the required features.  
Newer cards mainly improve resolution, filtering, and anti-aliasing.

---

## Below Minimum Specification

The following chipsets—and any cards based on them—are considered **below minimum spec**:

- 3dfx Voodoo 1, 2, 3 *(1,2 not supported; 3 poor image quality)*
- ATI Rage128, Rage Pro *(poor image quality)*
- Intel i740, i810 *(poor image quality)*
- Matrox G200, G400, G450 *(poor image quality)*
- nVidia Riva128 *(poor image quality)*
- S3 Savage 4, Savage 2000 *(particularly bad; may hang)*

See [Feature Lists](feature_lists.md) for an explanation of why these cards are not capable of producing good quality images in MiB64.

---

## Notes

You may find MiB64 usable on a lower-spec system than described here—especially with certain games and careful configuration.  
If so, enjoy—but please don’t expect too much.

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Minimum Specs Protocol Complete -->
