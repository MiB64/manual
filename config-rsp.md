---
title: RSP Config
nav_order: 11
---

<!-- This one is the best to use for all situations. -->        
<style>
.zoom-pair {
  display: flex;
  gap: 12px;
  align-items: flex-end;
  justify-content: flex-start;
  position: relative;
  margin-left: auto;
  margin-right: auto;
  width: max-content;
  text-align: left;
}

.zoom-on-hover {
  display: inline-block;
  position: relative;
}

.zoom-on-hover img {
  display: block;
  cursor: zoom-in;
  transition: transform 0.3s ease;
  position: relative;
  z-index: 1;
  transform-origin: left center;
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

/* Final fix for standalone zoomable images */
.zoom-single {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: max-content;
  text-align: center;
}

.zoom-single:hover img {
  transform: scale(1.5);
  transform-origin: center center;
  z-index: 999;
}
</style>

## <center><b>Internal RSP (Reality Signal Processor)</b></center>
<b>

<b>
<div class="zoom-pair">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/config_rsp.png" alt="RSP Config Dialog" width="300" height="214" />
  </div>
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/Internal_RSP.png" alt="Internal RSP" width="195" />
  </div>
</div>
<p style="text-align: center;"><strong>Hover to zoom</strong></p>

<!-- ClauseEcho: Interactive Images -->

Options > Configure Internal RSP

This page covers configuration of the Internal RSP.

## <center>Configure RSP</center>
<b>
<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/Internal_RSP.png" alt="Internal RSP" width="195" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Images -->

1. [Enable HLE Audio (If plugin supports it)](#o1)  
2. [Enable HLE Video (If plugin supports it)](#o2)  
3. [CPU core style](#o3)

---

### <a name="o1"></a>Enable HLE Audio (If plugin supports it)

- **Default setting**: disabled  
- **Recommended setting**: disabled

If disabled, the RSP will process Alists (provide low level emulated audio output). This generally provides good compatibility and quality.

If enabled, ALists are passed to the audio plugin (for high level emulation). This may provide better performance or extended capabilities, depending on your [choice of audio plugin](config-audio).

Changes take effect instantly.  
This setting is saved globally (in the registry) between sessions.

---

### <a name="o2"></a>Enable HLE Video (If plugin supports it)

- **Default setting**: disabled  
- **Recommended setting**: disabled

If enabled, Dlists will be passed to the video plugin (for high level emulation).  
This is not usually successful with the default plugin, although it does have some HLE compatibility if needed for slower or lower spec systems.

However, this is almost always the preferred solution for speed and quality with HLE video plugins.

If disabled, the RSP will process Dlists (provide low level emulated graphics output).  
This is not usually successful with the default plugin.

This is almost always the preferred solution for quality with the default plugin, but the cost will be speed on lower spec systems.

Changes take effect instantly.  
This setting is **not** saved between sessions.

---

### <a name="o3"></a>CPU core style

- **Default setting**: Recompiler  
- **Recommended setting**: Recompiler

If Recompiler is selected, the RSP will use a separate (low level) recompiling core.  
This provides far superior performance. In theory, the recompiler is slightly less compatible than the interpreter, but it has been improved in v1.5 to the point where there are no known limitations—so you should never need to use the interpreter!

If Interpreter is selected, the RSP will use a separate (low level) interpretive core.  
Performance is generally significantly lower. See above about compatibility.

**Tip**: If you do use the RSP interpreter for any reason, you are probably also going to want to use HLE audio to avoid a severe speed penalty.

Changes take effect instantly.  
This setting is saved globally (in the registry) between sessions.

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: RSP Config Protocol Activated -->
