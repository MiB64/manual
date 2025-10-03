---
title: Video (Graphics) Config
nav_order: 8
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

## <center>Configuration: Icepir8's Legacy LLE Graphics plugin</center>

<div class="zoom-pair">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/config_gfx2.png" alt="Config Video Dialog" width="300" height="217" />
  </div>
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/Icepir8sMiBLLE.png" alt="Config Icepir8s MiB LLE Plugin" width="150" />
  </div>
</div>
<p style="text-align: center;"><strong>Hover to zoom</strong></p>

<!-- ClauseEcho: Interactive Images -->

Options > Configure Graphics Plugin

Below all the tabs are three buttons, OK, Cancel and Apply. Hopefully the first two are self-explanatory - cancel closes discarding changes, OK closes keeping changes (but they aren't acutally written to file until you close MiB64. The Apply button is to allow you to see the effects of changes to graphics configuration in real time, while a game is running. This button does not save changes to file - saving to file is done on application exit. Therefore its a good idea to restart MiB64 once after making a lot of changes that you want to keep, just in case anything crashes.

<a href="#General:">General</a>

1. <a href="#g1">"Multithread rendering [Checkbox]"</a>  
2. <a href="#g2">"Threads - (0=auto)"</a>  
3. <a href="#g3">"Compatibilty"</a>  
4. <a href="#g4">"Capture Format"</a>

<a name="General:">General</a>

<a name="g1">"Multithread rendering [Checkbox]"</a>

- default setting: enabled  
- generally recommended setting: enabled

when enabled, it will use the amount of threads displayed in the <a href="#g2">"Threads"</a> section below.

If Multithread rendering is unchecked, the rendering speed will be very slow. When it is checked as it is by defualt, the speed is musch faster because multiple threads are used to render the graphics.

<a name="g2">"Threads - (0=auto)"</a>

- default setting: 0 =auto  
- generally recommended setting: 0

If 0 is used, it will automatically select the best amount of threads for your system to handle.will use multiple thread. You can also select your own amount that you input yourself to decide on the best for your system.

<a name="g3">"Compatibilty"</a>

- default setting: Moderate, some glitches  
- generally recommended setting: default.

There are three settings to choose from:

- Fast, most glitches  
- Moderate, some glitches (default)  
- Slow, most glitches.

Compatibility lets you select to trade compatibility for speed of rendering. If your system can handle the more compatible setting, use it. You can see the effect of this setting in the Intro for Mario Tennis when the trophy is shown. When less compatible mode is selected the highlights on the trophy are not correct.

<a name="g4">"Capture Format"</a>

- default setting: Png  
- generally recommended setting: Users choice.

There are three options to choose from:

- <a href="#PNG">Png (.png) - default</a>  
- <a href="#Bitmap">Bitmap (.bmp)</a>  
- <a href="#JPEG">Jpeg (.jpg)</a>

To take a screenshot you can use System>Screenshot Capture or F3 Shortcut when a gamne is running.

It is really up to the user to decide which format they prefer for Screenshots, but to help you decide we have broken them down for you to consider.

<a name="PNG">PNG</a> (.png) PNG or Portable Network Graphics files are a lossless image format. It was designed to replace gif format as gif supported 256 colors unlike PNG which support 16 million colors.

<a name="Bitmap">Bitmap</a> (.bmp) Bit Map Image file is developed by Microsoft for windows. It is same as TIFF due to lossless, no compression property. Due to BMP being a proprietary format, it is generally recommended to use TIFF files.

<a name="JPEG">JPEG</a> (.jpg, .jpeg) Joint Photographic Experts Group is a loss-prone (lossy) format in which data is lost to reduce the size of the image. Due to compression, some data is lost but that loss is very less. It is a very common format and is good for digital cameras, nonprofessional prints, E-Mail, Powerpoint, etc., making it ideal for web use.

<a name="Video_Interface:">Video Interface:</a>

<a name="vi1">"Window mode resolution"</a>

- default setting: 320x240  
- generally recommended setting: Users choice.

Here is where you chose you designed Emulation Window mode size. This is left to the requirementsto decide.

Window mode resolution is the size of the window used to display the graphics. The graphics are rendered at the native N64 resolution internally. If the two are different the internal graphics will be resized by your video card.

<a name="vi2">"Output Mode"</a>

- default setting: Filtered  
- generally recommended setting: Filtered

There are three settings to choose from:

- <a href="#Filtered">Filtered (default)</a>  
- <a href="#Unfiltered">Unfiltered</a>  
- <a href="#Depth">Depth</a>  
- <a href="#Coverage">Coverage</a>

<a name="Filtered">Filtered</a>, uses Interpolation when rendering to screen. Unfiltered don't use

<a name="Unfiltered">Unfiltered</a>, is basically the same as nearest neighbor Interpolation.

<a name="Depth">Depth</a>, outputs the depth buffer to the screen. closer objects are darker and further objects are lighter. Interesting but not useful for game play. This could be very useful if you are making a homebrew rom and are having perspective issues.

<a name="Coverage">Coverage</a>, shows what areas have been rendered to. It is interesting to see but it is not very useful.

<a name="vi3">"Interpolation"</a>

- default setting: Nearest-neighbour  
- generally recommended setting: default.

This the method your video card will use to resize the image when resizing.

There are two settings to choose from:

- <a href="#Nearest-neighbour">Nearest-neighbour (default)</a>  
- <a href="#Linear">Linear</a>

<a name="Nearest-neighbour">Nearest-neighbour</a> (default), is the fastest. Unless you are using a very low power video card it will not be noticeable.

<a name="Linear">Linear</a>, uses bi-linear scaling to smooth the image as it resizes the output image. This looks better and is the recommended setting.

<a name="vi4">"16:9 widescreen" [Checkbox]</a>

- default setting: disabled  
- generally recommended setting: Users choice.

This forces the video resolution to 16:9 widescren, especially useful is the original screen is from a PAL region of 4:3.

<a name="vi5">"Hide Overscans" [Checkbox]</a>

- default setting: disabled  
- generally recommended setting: Users choice.

This does what it says on the tin to coin a phrase. To hide or not to hide? To help you decide, we have given a description as to what Overscan is to assist you.

"Overscan" is the term used to describe the practice of TVs hiding the extreme edges of the picture they receive. In old CRT TVs this was because the edge of the tube would have produced a bad image, so the viewable area was reduced. This has since become a broadcast standard so there is often garbage and computer signals carried on the border of television broadcasts, so even HDTVs presume these extreme edges should be hidden.

<a name="vi6">"Exclusive fullscreen" [Checkbox]</a>

- default setting: disabled  
- generally recommended setting: Users choice.

Ice can explain this option in detail for advantages and benifits.

<a name="vi7">"Enable VSync" [Checkbox]</a>

- default setting: enabled  
- generally recommended setting: Users choice.

What is VSync? To help you we have described it below for for you to add up the Pro and Cons so you can decide.

VSync (Vertical Synchronisation), Is the process of timing a graphics card sends each frame to wait until the monitor is ready to start drawing the next frame (this is not necessary - the graphics card can updated frames at any stage during the cycle, which causes image tearing as two consecutive frames are shown at once, the top of one and the bottom of the other). A MiB64 video plugin option (display tab), also system dependant. There are advantages and disadvantages to using Vertical Sync.

When Enable VSync is checked, rendering speed can be impacted. If a frame finishes just after VSync occurs the plugin has to wait for the next VSync to display the frame. This adds time to render frames. Some roms this is very noticeable effect.

Settings from the plugin are saved globally, in the Icepir8LLE-config.ini file.

<a href="#">Return to the top</a>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: MiB64 Config Video Protocol Complete -->
