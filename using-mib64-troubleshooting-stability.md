---
title: Troubleshooting Stability
nav_order: 7
parent: Using MiB64
---

## <center>Troubleshooting stability problems</center>

Stability problems can be broadly broken down into four categories, reflecting the complex nature of an emulator:

1. [System](#o1)  
2. [Application](#o2)  
3. [Game](#o3)  
4. [Speed](#o4)

### <a name="o1"></a>System failures

This type of problem refers to a complete lock up of your PC or an operating system STOP error (BSOD), usually requiring a hard reset of the system.

There are no known bugs in MiB64 (we cannot vouch for 3rd party plugins, of course) that would cause a system crash/lockup/other form of operating system failure. If you experience such a problem while using MiB64, it is very likely that you have a hardware or driver or DirectX or operating system problem. Run diagnostic software and check that your system is stable in other Direct3D applications, games, benchmark utilities etc. Find some torture-testing utilities. Consult hardware documentation if you need further help. You could try changing plugins, and use dummy plugins to see if you can narrow down to one area that's causing the problem (doesn't mean it's necessarily a fault in that area of the emulator, but that area of the complete system).

- Check that other applications are not leaving your system (particularly video and DirectX) in an unusable state, by starting the OS with no other applications.
- Check that the problem is not bad drivers, for example we have seen STOP errors being caused by drivers from a specific hardware company – use MiB64 on any other company's hardware and in the same situation it works fine. Contact the appropriate organisation for technical support.

### <a name="o2"></a>Application failures

This type of problem refers to an actual crash or hang in the MiB64 application, resulting in a generic Windows error message "this program has performed an illegal operation" or "this program is not responding" etc. The exact type of message depends on your version of Windows, but the point is that you are seeing a Windows error message not a MiB64 error message – in other words, MiB64 has failed to handle an error, which could indicate a bug in MiB64 or a system failure:

- Are you running a supported game with the correct Game settings? A small number of games can cause MiB64 to fail under some conditions.
- Is your hardware OK? Memory problems, overclocking etc. can cause applications to fail.

### <a name="o3"></a>Game failures

This type of error refers to an error in the MiB64 application or plugin(s) that is handled successfully by the application or plugin error handlers. A good example of this is the "UnHandled OpCode" error (OK, the OpCode itself is unhandled, but the situation is handled – you can end emulation, reboot the game, or play another game, without MiB64 crashing). Another example is a graphics Access Violation. This type of error nearly always indicates a bug or a configuration error in the emulator.

- Are you running a supported game with the correct Game settings? Almost any game will crash without the correct configuration.
- Anything you can do to improve **core security** ([Game Settings](app_rom_settings.html)) may prevent the problem.

### <a name="o4"></a>Troubleshooting speed problems

The first thing to understand is what speed to expect from MiB64 – as a rough guide, the following specifications should be *just* fast enough for each game at full speed with the default configuration:

- Mario64 – P2-450MHz  
- Zelda – Athlon 800MHz  
- Perfect Dark – Athlon 1.2GHz

**Points:**

1. Not all the suggestions below will improve performance *for you*. Some will only reduce quality, stability etc. You have to try them and see the effects for yourself.
2. Some of these suggestions have the potential to do damage to your hardware or software or data or all three. Any such damage that results from your following the suggestions listed on this page is entirely your own responsibility – take care and don't do anything you are not confident you understand – seek advice from hardware internet sites etc. if you need to.
3. As a general rule, **FPS in MiB64 depends on your CPU, not your graphics card**, because most users are CPU limited, not graphics card limited, but the graphics card can become the limiting factor at high resolutions with high levels of FSAA, or if you have a below [minimum spec](min_spec.html) graphics card.
4. The generally **most significant factors are listed first**, descending to the least significant (i.e. the most to the least likely to help, in my opinion and experience).

Check problem is not being caused by one of your plugins – plugins can stall the emulator by design or due to bugs in their coding.

#### Hardware level

1. increase CPU clock rate or upgrade CPU  
2. increase front side bus/RAM clock rate  
3. add RAM if you are short*  
4. choose a CPU with SSE (& MMX!) capability  
5. adjust RAM timings, cache timings etc.*  
6. increase graphics card clock rates*  
7. use PCI rather than ISA sound card  
8. disable any unneeded ports/hardware  
9. avoid IRQ sharing*  
10. use USB rather than Gameport input devices

#### Driver level

1. update drivers, video card drivers, chipset drivers, sound drivers*  
2. use 16 bit colour desktop rather than 24/32*  
3. use lower level of anti-aliasing, or none at all*  
4. disable Vsync  
5. disable multi-display if your system supports it*  
6. use 16 bit z buffer (rather than 24/32)*  
7. use texture compression*  
8. lower or raise monitor refresh rate*

#### Operating System level

1. shut down all non-essential (background) processes  
2. disable findfast/file indexing/system restore/task scheduler etc.  
3. adjust process priorities  
4. use Win2K/XP series OS if you have enough RAM (192MB+)  
5. use Win98SE if you don't have enough RAM (WinME seems generally a bad choice)  
6. update DirectX version  
7. just rebooting Windows can help free resources  
8. clean reinstall Windows in extreme problem cases  
9. compact memory  
10. fix pagefile size  
11. move pagefile to fastest drive*  
12. defragment hard drive  
13. lower debug levels on DirectX  
14. don't use debug (usually beta) builds of drivers or DirectX

#### Application level

1. don't run [multiple instances](multiple_instances.html) of MiB64  
2. fullscreen modes may be considerably faster than windowed modes*

#### Emulator core

1. use [Recompiler](app_rom_settings.html#o1) instead of Interpreter**  
2. disable Limit FPS – System > Limit FPS  
3. enable [Register Caching](app_rom_settings.html#r5)**  
4. enable [Advanced Block Linking](app_rom_settings.html#r2)**  
5. enable [Larger Compiler Buffer](app_rom_settings.html#r3)**  
6. use less secure [method to handle self-modifying code](pp_rom_settings.html#r1)**  
7. don't enable the [expansion pack](app_rom_settings.html#o2) if it's not needed**  
8. [state saving and loading](save_load_games.html) sometimes helps the recompiler**  
9. disable [TLB](app_rom_settings.html#o7) (but only if not needed!)**

#### Plugins

1. use the RSP recompiler core rather than interpreter core  
2. don't use any form of Framebuffer emulation  
3. don't enable Audio Sync on either audio plugin  
4. use a lower resolution  
5. use 16 bit colour modes rather than 24/32  
6. if you want true colour, use 32 bit rather than 24*

\* effectiveness depends on system (hardware)  
\*\* effectiveness depends on game

---

<!-- Footer Navigation Block -->

<table align="center" style="width: 80%">
  <tr>
    <td style="text-align: center"><a href="using-mib64">Using MiB64</a></td>
    <td style="text-align: center"><a href="start-stop-reset-games">Start, Stop, Reset Games</a></td>
    <td style="text-align: center"><a href="save-load-games">Save & Load Games</a></td>
    <td style="text-align: center"><a href="/manual/manual/manual/cheats">Using Cheats</a></td>
  </tr>
  <tr>
    <td style="text-align: center"><a href="taking-screenshots">Taking Screenshots</a></td>
    <td style="text-align: center"><a href="multiple-instances">Multiple Instances</a></td>
    <td style="text-align: center"><a href="keyboard-shortcuts">Keyboard Shortcuts</a></td>
    <td style="text-align: center"><a href="using-mib64-troubleshooting-stability">Troubleshooting Stability</a></td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Troubleshooting Stability Protocol Activated -->
