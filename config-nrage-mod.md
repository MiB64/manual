---
title: Modifiers Config
nav_order: 3
parent: Input (Controller) Config
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

## <center><b>N-Rage MiB64 Input Configuration — Modifiers Tab</b></center>
<b>

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_MiB64_Input_Modifiers.png" alt="Modifiers Tab" width="320" height="224" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

<!-- ClauseEcho: Interactive Image -->

This tab can be a bit confusing, but allows you to do very powerful things once you figure it out.

At first, everything will be grayed out except **New Modifier** and **Delete Modifier**. Let's start by playing around a bit.

**New Modifier** creates a modifier, obviously. So let's try that. Click it once. Now select the modifier you've just created. The right half labelled **Adjust Modifier** should activate to let you know you've selected a modifier. It should look like this:

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_MiB64_Input_Modifiers_None.png" alt="Modifiers Tab" width="320" height="224" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

Okay, we've got a modifier, but it's not assigned to any key and it doesn't do anything. Let's take a look at what we can change.

First off, there's the **Assign Mod** button. This lets us bind a key to the modifier. It works exactly like binding a button in the Controls tab.

Then there's **Mod Type**, which is now set to "None". This lets you select different types of modifiers; we'll get into this shortly.

To the right of that is a checkbox marked "Toggle". If this is unchecked, the modifier will only activate as long as the button is held down. If it is checked, one press of the button will activate it and the next will deactivate it.

Below that is the **Apply Changes** button. **If you change anything in the Adjust Modifier panel, you must click Apply Changes for the changes to take effect.** Before selecting another modifier, or selecting another tab, or clicking Save, make sure that you've applied the changes! When you apply changes, the list of modifiers will update to let you know that the changes took effect.

**Reset** will revert all changes to the modifier since you've pressed the "Apply Changes" button. It has the same effect as deselecting the modifier from the list and selecting it again.

Here are the types of Modifiers and what they do:

**Movement** — lets you set a multiplier for analog stick movements, or invert axes  
**Macro** — lets you press multiple N64 buttons and/or axes with one input, and also lets you create rapid-fire buttons  
**Configuration** — lets you change N64 analog stick configurations. You can switch between Config 1 and Config 2 (from the Controls tab). The "Switch ?-Mode" under "Mouse" switches between Buffered and Absolute mouse modes (under Devices), and the "Switch ?-Mode" under "Keyboard" toggles Absolute Keyboard modes.

Let's try something. Select the new modifier that we created before. Assign the modifier to the "Shift" key, set the mod type to Configuration, and toggle the "Switch X-mode" and "Switch Y-mode" buttons. *Now hit Apply Changes.* If you've done it right, the modifier in the list should change to match, and it should look like this:

<div style="text-align: center;">
  <div class="zoom-on-hover">
    <img src="/manual/asset/images/NRage_MiB64_Input_Modifiers_Config.png" alt="Modifiers Tab" width="320" height="224" />
  </div>
  <p><strong>Hover to zoom</strong></p>
</div>

What we've done is created a modifier that when held down will change the mouse mode from Buffered to Absolute, and when released will change it back. I use this modifier (along with the R-trigger assigned to the same Shift key) in *Perfect Dark*, so that when I hold down the "aim" key I can use the mouse to target a point on the screen. It makes sniping a breeze.

Modifiers let you do things like bind a keyboard key AND a gamepad button to the same N64 button (bind one in Controls and create a Macro Modifier for the other). There are no limits on how many modifiers you can have bound to a single key or button, but you are limited to a maximum of 255 modifiers total per controller. There are a lot of things you can do with modifiers, and I'll leave it up to you to experiment!

<table align="center">
  <tr>
    <td style="text-align: center;"><a href="config-nrage-controls">Controls</a></td>
    <td style="text-align: center;"><a href="config-nrage-devices">Devices</a></td>
    <td style="text-align: center;"><a href="config-nrage-mod">Modifiers</a></td>
    <td style="text-align: center;"><a href="config-nrage-controller-pak">Controller Pak</a></td>
  </tr>
  <tr>
    <td style="text-align: center;"><a href="config-nrage-trouble-rumble">Rumble Troubleshoot</a></td>
    <td style="text-align: center;"><a href="config-nrage-faq">General FAQ</a></td>
    <td style="text-align: center;"><a href="config-nrage-shortcuts">Shortcuts</a></td>
    <td style="text-align: center;">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Modifiers Config Protocol Activated -->
