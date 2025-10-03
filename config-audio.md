---
title: Audio (Sound) Config
nav_order: 9
---

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

## <center>Configuration: Azimer's Legacy Audio Plugin</center>
<b>
<div class="zoom-pair">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/config_audio.png" alt="Config Audio Dialog" width="300" height="214" />
  </div>
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/azi1.png" alt="Azi Dialog" width="300" height="214" />
  </div>
</div>
<p style="text-align: center;"><strong>Hover to zoom</strong></p>

<!-- ClauseEcho: Interactive Images -->

Options > Configure Audio Plugin

## <center>Settings Tab</center>
<b>
<div style="text-align: center;">
  <div class="zoom-on-hover">
  <img src="/manual/asset/images/azi1.png" alt="Settings Tab" width="300" height="214" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Images -->

This page covers configuration of the default MiB64 audio plugin — Azimer's Legacy Audio 0.70.10.

<ol>
  <li><a href="#o1">"Game Profile"</a></li>
  <li><a href="#o2">"Output Devices"</a></li>
  <li><a href="#o3">"Backend Sound Driver"</a></li>
  <li><a href="#o4">"Volume"</a></li>
  <li><a href="#o5">"Mute"</a></li>
</ol>

Points:

- The audio plugin does not include an audio emulator! It must be used in conjunction with the RSP plugin.  
- The RSP plugin must be configured with "send Audio Lists to Audio Plugin" disabled or the audio plugin will receive no audio data and hence you will hear no sound!

<a name="o1"><strong>"Game Profile"</strong></a>

This setting is disabled (greyed out) and serves no function currently.

<a name="o2"><strong>"Output Devices"</strong></a>

This enables you to output the sound to whatever device may be listed in the dropdown list of available devices.

<a name="o3"><strong>"Backend Sound Driver"</strong></a>

<div class="zoom-on-hover" style="text-align: center;">
  <img src="/manual/asset/images/azi2.png" alt="Advanced Tab" width="300" height="214" />
  <p><strong>Hover to zoom</strong></p>
</div>

<ul>
  <li>DirectSound 8 Driver — Recommended default for Windows XP</li>
  <li>DirectSound 8 Legacy Driver — Use only if DirectSound 8 does not work properly</li>
  <li>No Sound Driver — Recommended if you do not have sound</li>
  <li>WASAPI Driver (experimental) — Recommended for Windows Vista or better</li>
  <li>WaveOut Driver — Not Recommended but most Windows compatible</li>
  <li>XAudio 2 Driver (default setting) — Recommended fallback when WASAPI is not available</li>
  <li>XAudio 2 Legacy Driver — Not Recommended</li>
</ul>

By default the XAudio2 Driver is selected. But the user can use any option via a dropdown menu.

<a name="o4"><strong>"Volume"</strong></a>

- default setting: 50%  
- generally recommended setting: user preference

Its function should be fairly obvious. You can use the Up and Down arrows, Page Up and Page Down keys, and Mousewheel as shortcuts. Setting all the way down is equivalent to muting the emulator.

This setting is global (applies to all ROMs), takes effect instantly, and is saved in the AziCfg.bin.

<a name="o5"><strong>"Mute"</strong></a>

This checkbox is a simple toggle to mute or unmute sound.

<ul>
  <li>Check to Mute</li>
  <li>Un-check will return to original position when dialog is still open</li>
</ul>

If you mute and then click OK and close, when you next load and un-check, it will still be on zero. Use the volume slider to adjust the volume once again to your desired setting.

## <center>Advanced_Tab</center>
<b>
<div style="text-align: center;">
  <div class="zoom-on-hover">
  <img src="/manual/asset/images/azi3.png" alt="Advanced Tab" width="300" height="214" />
  </div>
  <p><strong>Hover to zoom</strong></p></div>

<!-- ClauseEcho: Interactive Images -->

<a href="#Buffer_Options:">Buffer Options:</a>

<ul>
  <li><a href="#Prevent_Buffer_Overruns">Prevent Buffer Overruns (Checkbox)</a></li>
  <li><a href="#Force_Old_Audio_Sync">Force Old Audio Sync (Checkbox)</a></li>
  <li><a href="#Buffer_FPS">Buffer FPS (Slider)</a></li>
  <li><a href="#Backend_FPS">Backend FPS (Slider)</a></li>
  <li><a href="#Buffers">Buffers (Slider)</a></li>
</ul>

<a href="#Emulation_Options">Emulation Options:</a>

<ul>
  <li><a href="#Emulate Audio Interface">Emulate Audio Interface (Checkbox)</a></li>
</ul>

<a href="#Playback_Tweaks">Playback Tweaks:</a>

<ul>
  <li><a href="#Frequency">Frequency (Greyedout)</a></li>
  <li><a href="#Disallow Thread  Yielding DSB">Disallow Thread Yielding DSB (Checkbox)</a></li>
  <li><a href="#Disallow Thread  Yielding XA2">Disallow Thread Yielding XA2 (Checkbox)</a></li>
</ul>

<h3><a name="Buffer_Options:"><em>Buffer Options</em></a></h3>

<a name="Prevent_Buffer_Overruns"><strong>"Prevent Buffer Overruns (Checkbox)"</strong></a>

This will cause the emulation thread to slow down when the audio buffer overruns. It will pause the thread until the buffer isn't full.

<a name="Force_Old_Audio_Sync"><strong>"Force Old Audio Sync (Checkbox)"</strong></a>

This will cause the emulation thread to slow down when the audio buffer overruns. This is different from overrun as it will copy the entirety of the buffer into output locking the thread until it is able to.

<a name="Buffer_FPS"><strong>"Buffer FPS (Slider)"</strong></a>

The number of milliseconds (frames) to buffer audio in the secondary buffer.

<a name="Backend_FPS"><strong>"Backend FPS (Slider)"</strong></a>

The number of milliseconds (frames) to buffer audio in the primary buffer (API level).

<a name="Buffers"><strong>"Buffers (Slider)"</strong></a>

The number of buffers available to buffer the audio.

<h3><a name="Emulation_Options"><strong><em>Emulation Options</em></strong></a></h3>

<a name="Emulate Audio Interface"><strong>"Emulate Audio Interface (Checkbox)"</strong></a>

This setting is disabled (greyed out) and serves no function currently. Emulate Audio Interface will always be enabled and will only be skipped when the emulator does its own audio emulation.

<h3><a name="Playback_Tweaks"><strong><em>Playback Tweaks</em></strong></a></h3>

<a name="Frequency"><strong>"Frequency (Greyedout)"</strong></a>

This setting is disabled (greyed out) and serves no function currently.

<a name="Disallow Thread  Yielding DSB"><strong>"Disallow Thread Yielding DSB (Checkbox)"</strong></a>

A hack used to prevent the yielding of the audio thread for DirectSound8. This may smooth out audio issues.

<a name="Disallow Thread  Yielding XA2"><strong>"Disallow Thread Yielding XA2 (Checkbox)"</strong></a>

A hack used to prevent the yielding of the audio thread for XAudio2. This may smooth out audio issues.

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Config Audio Protocol Complete -->
