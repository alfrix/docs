# PlayStation (Beetle PSX HW)

## Background

Enhanced port of standalone Mednafen PSX to libretro.

### Why use this core?

Awaiting description.

### Authors

- Mednafen Team

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_psx_hw.md). Changes are proposed using "Pull Requests."

## See also

- [PlayStation (Beetle PSX)](https://doc.libretro.com/library/beetle_psx/)
- [PlayStation (PCSX ReARMed)](https://doc.libretro.com/library/pcsx_rearmed/)

## License

GPLv2

## Extensions

Content that can be loaded by the Beetle PSX HW core have the following file extensions:

- .cue
- .toc
- .m3u
- .ccd
- .exe
- .pbp
- .chd

## Databases

RetroArch database(s) that are associated with the Beetle PSX HW core:

- [Sony - PlayStation](https://github.com/libretro/libretro-database/blob/master/rdb/Sony%20-%20PlayStation.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

|   Filename   | Description                    |              md5sum              |
|:------------:|:------------------------------:|:--------------------------------:|
| scph5500.bin | PS1 JP BIOS - Required for JP  | 8dd7d5296a650fac7319bce665a6a53c |
| scph5501.bin | PS1 US BIOS - Required for US  | 490f666e1afb15b7362b406ed1cea246 |
| scph5502.bin | PS1 EU BIOS - Required for EU  | 32736f17079d0b2b7024407c39bd3050 |

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| RetroAchievements | ✕         |
| RetroArch Cheats  | ✔         |
| Native Cheats     | ✕         |
| Controllers       | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | -         |
| Rumble            | ✔         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| Softpatching      | -         |

The Beetle PSX HW core's directory name is 'Beetle PSX HW'

- Game data is saved/loaded to and from where save files are stored.
- Save states are saved/loaded to and from where state files are stored.

### Loading content

Beetle PSX HW needs a cue-sheet that points to an image file. A cue sheet, or cue file, is a metadata file which describes how the tracks of a CD or DVD are laid out.

If you have e.g. `foo.bin`, you should create a text file and save it as `foo.cue`. Most PS1 games are single-track, so the cue file contents should look like this:

`foobin.cue`
```
 FILE "foo.bin" BINARY
  TRACK 01 MODE1/2352
   INDEX 01 00:00:00
```

After that, you can load the `foo.cue` file in RetroArch with the Beetle PSX HW core.

!!! warning ""
    Certain PS1 games are multi-track, so their .cue files might be more complicated.
	
#### Playing PAL copy protected games

PAL copy protected games need a SBI Subchannel file next to the bin/cue files in order to get past the copy protection.

- Ape Escape (Europe).bin
- Ape Escape (Europe).cue
- **Ape Escape (Europe).sbi**

!!! warning ""
	For proper PAL game compatibility, the 'Skip BIOS' core option needs to be set to off.

### Multiple-disk games

If foo is a multiple-disk game, you should have .cue files for each one, e.g. `foo (Disc 1).cue`, `foo (Disc 2).cue`, `foo (Disc 3).cue`.

To take advantage of Beetle PSW HW's Disk Control feature for disk swapping, an index file (a m3u file) should be made.

Create a text file and save it as `foo.m3u`. Then enter your game's .cue files on it. The m3u file contents should look something like this:

`foo.m3u`
```
foo (Disc 1).cue
foo (Disc 2).cue
foo (Disc 3).cue
```

After that, you can load the `foo.m3u` file in RetroArch with the Beetle PSX HW core.

Here's another m3u example done with Valkryie Profile

![m3u_example](images\Cores\beetle_psx_hw\m3u_example.png)

!!! warning ""
	Adding multi-track games to a RetroArch playlist is recommended. (Manually add an entry a playlist that points to `foo.m3u`)

### Game compression

Alternatively to using cue sheets with .bin files, you can convert your games to .pbp (Playstation Portable update file) to reduce file sizes and neaten up your game folder. A recommended .pbp convert tool is PSX2PSP.

If converting a multiple-disk game, all disks should be added to the same .pbp file, rather than making a .m3u file for them.

Most conversion tools will want a single .bin file for each disk. If your game uses multiple .bin files (tracks) per disk, you will have to mount the cue sheet to a virtual drive and re-burn the images onto a single track before conversion.

!!! warning ""
    RetroArch does not currently have .pbp database due to variability in users' conversion methods. All .pbp games will have to be added to playlists manually.

### Saves

For game savedata storage, the PSX console used memory cards. The PSX console had two slots for memory cards. 

In this doc, the first memory card slot will be referred to as 'Memcard slot 0' and the second slot will be referred to as 'Memcard slot 1'.

For memory card functionality and usage, the Beetle PSX HW core will either use the Libretro savedata format or the Mednafen savedata format.

<center>

| Libretro savedata format   |  Mednafen savedata format        |
|----------------------------|----------------------------------|
| gamename.srm               |   gamename.slot#.mcr             |

</center>

**By default**, the Beetle PSX HW core will use Libretro's savedata format for Memcard slot 0 and Mednafen's savedata format for Memcard slot 1.

<center>

| Memcard slot 0 | Memcard slot 1 |
|----------------|----------------|
| gamename.srm   | gamename.1.mcr |

</center>

!!! warning ""
    Memory card behavior can be controlled with the following [core options](https://buildbot.libretro.com/docs/library/beetle_psx/#core-options) (Memcard 0 method, Enable memory card 1, Shared memcards).

**By default**, the filenames of the Memcard savedata will match the loaded cue or m3u or pbp filename, like this:

- Loaded content: Breath of Fire III (USA).cue

- **Memcard slot 0: Breath of Fire III (USA).srm**

- **Memcard slot 1: Breath of Fire III (USA).1.mcr**

or

- Loaded content: Final Fantasy VII (USA).m3u

- **Memcard slot 0: Final Fantasy VII (USA).srm**

- **Memcard slot 1: Final Fantasy VII (USA).1.mcr**

or

- Loaded content: Wild Arms 2 (USA).pbp

- **Memcard slot 0: `Wild Arms 2 (USA).srm**

- **Memcard slot 1: `Wild Arms 2 (USA).1.mcr**

!!! warning ""
	To import your old memory cards from other emulators, you need to rename them to either the Libretro savedata format or the Mednafen savedata format.
	
### Rumble

Rumble only works when the corresponding user's device type is set to **DualShock** and the joypad input driver being used has rumble function implementation (e.g. **Xinput**).

## Core options

*The Beetle PSX HW core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.*

- **Renderer (restart)** (**vulkan**/opengl/software): Choose which video renderer will be used. **Software is the most accurate renderer.** The OpenGL and Vulkan renderers will enable and/or speedup enhancements like upscaling and texture filtering. **The OpenGL and Vulkan renderers must be used with it's corresponding video driver in RetroArch's Driver settings.** **Also, Hardware Shared Context must be enabled in RetroArch's Core settings.**
- **Software framebuffer** (Off/**On**): If off, the software renderer will skip some steps. Potential speedup. Causes bad graphics when doing framebuffer readbacks.
- **Adaptive smoothing** (Off/**On**): When upscaling, smooths out 2D elements while keeping 3D elements sharp. Only for the Vulkan renderer at the moment.

??? note "*Adapative smoothing - Off*"
    ![adaptive_smoothing_off](images\Cores\beetle_psx_hw\adaptive_smoothing_off.png)

??? note "*Adaptive smoothing - On*"
    ![adaptive_smoothing_on](images\Cores\beetle_psx_hw\adaptive_smoothing_on.png)

- **Internal GPU resolution** (**1x(native)**/2x/4x/8x/16x/32x): Modify the resolution.

??? note "*Internal GPU Resolution - 1x*"
    ![internal_gpu_resolution_1](images\Cores\beetle_psx_hw\internal_gpu_resolution_1.png)

??? note "*Internal GPU Resolution - 2x*"
    ![internal_gpu_resolution_2](images\Cores\beetle_psx_hw\internal_gpu_resolution_2.png)

- **Texture filtering** (**nearest**/SABR/xBR/bilinear/3-point/JINC2): Per-texture filtering. Only for the OpenGL renderer at the moment.

??? note "*nearest*"
    ![nearest](images\Cores\beetle_psx_hw\nearest.png)

??? note "*SABR*"
    ![SABR](images\Cores\beetle_psx_hw\SABR.png)

??? note "*xBR*"
    ![xBR](images\Cores\beetle_psx_hw\xBR.png)

??? note "*bilinear*"
    ![bilinear](images\Cores\beetle_psx_hw\bilinear.png)

??? note "*3-point*"
    ![3-point](images\Cores\beetle_psx_hw\3-point.png)

??? note "*JINC2*"
    ![JINC2](images\Cores\beetle_psx_hw\JINC2.png)

- **Internal color depth** (**dithered 16bpp (native)**/32bpp): PSX had 16bpp depth, Beetle PSX HW can go up to 32bpp. **Only for the OpenGL and Vulkan renderers at the moment.** The Vulkan renderer always uses 32bpp.
- **Wireframe mode** (**Off**/On): Shows only the outlines of polygons. Only for the OpenGL renderer. **For debug use.**

??? note "Wireframe mode - On"
	![wireframe_mode_on](images\Cores\beetle_psx_hw\wireframe_mode_on.png)

- **Display full VRAM** (**Off**/On): Everything in VRAM is drawn on screen. **For debug use.**

??? note "Display full VRAM - On"
	![display_full_vram_on](images\Cores\beetle_psx_hw\display_full_vram_on.png)

- **PGXP operation mode** (**Off**/memory only/memory + CPU): When on, floating point coordinates will be used for vertex positions, to avoid the PSX polygon jitter. 'memory + cpu' mode can further reduce jitter at the cost of performance and geometry glitches.
- **PGXP vertex cache** (**Off**/On): Maintains a cache for vertices. May result in better performance but can result in graphics glitches in most games.
- **PGXP perspective correct texturing** (**Off**/On): Original PSX did affine texture mapping, resulting in e.g. crooked lines across walls. This fixes it.
- **Widescreen mode hack** (**Off**/On): If on, renders in 16:9. Works best on 3D games.

??? note "Widescreen mode hack - Off"
	![widescreen_mode_hack_off](images\Cores\beetle_psx_hw\widescreen_mode_hack_off.png)
	
??? note "Widescreen mode hack - On"
	![widescreen_mode_hack_on](images\Cores\beetle_psx_hw\widescreen_mode_hack_on.png)

- **Frame duping (speedup)** (**Off**/On): Redraws/reuses the last frame if there was no new data.
- **CPU Overclock** (**Off**/On): Gets rid of memory access latency and makes all GTE instructions have 1 cycle latency.
- **Skip BIOS** (**Off**/On): Self-explanatory. **Some games have issues when this core option is enabled (Saga Frontier, PAL copy protected games, etc).** 

??? note "Skip BIOS - Off"
	![skip_bios_off](images\Cores\beetle_psx_hw\skip_bios_off.png)

- **Dithering pattern** (**1x(native)**/internal resolution/Off): If off, disables the dithering pattern the PSX applies to combat color banding. **Only for the OpenGL and Vulkan renderers. Vulkan always disables the pattern.**
- **Display internal FPS** (**Off**/On): Shows the frame rate at which the emulated PSX is drawing at. **Onscreen Notifications must be enabled in the RetroArch Onscreen Display Settings.**

??? note "Display internal FPS - On"
	![display_internal_fps_on](images\Cores\beetle_psx_hw\display_internal_fps_on.png)

- **Initial scanline** (0 to 40 in increments of 1. **0 is default**):  Sets the first scanline to be drawn on screen.
- **Last scanline** (210 to 239 in increments of 1. **239 is default**): Sets the last scanline to be drawn on screen.
- **Initial scanline PAL** (0 to 40 in increments of 1. **0 is default**): Sets the first scanline to be drawn on screen for PAL systems.
- **Last scanline PAL** (260 to 287 in increments of 1. **287 is default**): Sets the last scanline to be drawn on screen for PAL systems.
- **Crop Overscan** (Off/**On**): Crop out the potentially random glitchy video output that would have been hidden by the bezel around the edge of a standard-definition television screen.

??? note "Crop Overscan - On"
	![crop_overscan_on](images\Cores\beetle_psx_hw\crop_overscan_on.png)
	
??? note "Crop Overscan - Off"
	![crop_overscan_off](images\Cores\beetle_psx_hw\crop_overscan_off.png)

- **Additional Cropping** (**Off**/1 px/2 px/3 px/4 px/5 px/6 px/7 px/8 px): Self-explanatory.
- **Offset Cropped Image** (**Off**/1 px/2 px/3 px/4 px/-4 px/-3 px/-2 px/-1 px): Self-explanatory.
- **Analog self-calibration** (**Off**/On): When enabled, monitors the max values reached by the input, using it as a calibration heuristic which then scales the analog coordinates sent to the emulator accordingly. For best results, rotate the sticks at max amplitude for the algorithm to get a good estimate of the scaling factor, otherwise it will adjust while playing.
- **DualShock Analog button toggle** (**Off**/On): Toggles the Analog button from DualShock controllers, if disabled analogs are always on, if enabled you can toggle their state by pressing and holding START+SELECT+L1+L2+R1+R2.
- **Port 1: Multitap enable** (**Off**/On): Enables/Disables multitap functionality on port 1.
- **Port 2: Multitap enable** (**Off**/On): Enables/Disables multitap functionality on port 2.
- **Gun Cursor** (**Cross**/Dot/Off): Choose the cursor for the 'Guncon / G-Con 45' and 'Justifier' Device Types. Setting it to off disables the crosshair.

??? note "Gun Cursor - Cross"
	![cursor_cross](images\Cores\beetle_psx_hw\cursor_cross.png)
	
??? note "Gun Cursor - Dot"
	![cursor_dot](images\Cores\beetle_psx_hw\cursor_dot.png)	

??? note "Gun Cursor - Off"
	![cursor_off](images\Cores\beetle_psx_hw\cursor_off.png)		
	
- **Gun Trigger** (**Left Mouse Button**/Right Mouse Button): Select whether the left or right mouse button is used as the trigger for the 'Guncon / G-Con 45' and 'Justifier' Device Types. Look below at the [Controllers graph](https://buildbot.libretro.com/docs/library/beetle_psx_hw/#controllers-graph) section for more information.
- **Mouse Sensitivity** (5% to 200% in increments of 5%. **100% is default**): Configure the 'Mouse' Device Type's sensitivity.
- **CD Access Method (restart)** (**sync**/async/precache): Awaiting description.
- **Memcard 0 method** (**libretro**/mednafen): Choose the savedata format used for Memcard 0 (libretro or mednafen). Look above at the [Saves](https://buildbot.libretro.com/docs/library/beetle_psx_hw/#saves) for an explanation regarding the libretro and mednafen formats.
- **Enable memory card 1** (Off/**On**): Enable or disables Memcard slot 1. When disabled, games cannot save/load to Memcard slot 1.  **Memcard 1 must be enabled for game 'Codename Tenka'.**
- **Shared memcards (restart)** (**Off**/On): Games will share and save/load to the same memory cards.

<center>

| Memcard slot 0                     | Memcard slot 1                     |
|------------------------------------|------------------------------------|
| mednafen_psx_libretro_shared.0.mcr | mednafen_psx_libretro_shared.1.mcr |

</center>

!!! warning ""
	The 'Memcard 0 method' core option needs to be set to 'mednafen' for the 'Shared memcards' core option to function properly.

- **Increase CD loading speed** (**2x (native)**/4x/6x/8x/10x/12x/14x): An **experimental** feature, may not work correctly in all games. Can greatly reduce the loading times on games.

## Controllers

The Beetle PSX HW core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):

### User 1 - 8 Device Type(s)

- [**PlayStation Controller**](https://en.wikipedia.org/wiki/PlayStation_Controller) - Joypad - PlayStation Controller (SCPH-1080)

- [DualShock](https://en.wikipedia.org/wiki/DualShock) - Joypad - DualShock (SCPH-1200)

- [Analog Controller](https://en.wikipedia.org/wiki/Dual_Analog_Controller) - Joypad - PlayStation Dual Analog Controller(SCPH-1180)

- [Analog Joystick](https://en.wikipedia.org/wiki/PlayStation_Analog_Joystick) - Joypad - PlayStation Analog Joystick (SCPH-1110)

- [Guncon / G-Con 45](https://en.wikipedia.org/wiki/GunCon) - Lightgun - Namco Gun Controller (SLEH-00007)

- [Justifier](https://en.wikipedia.org/wiki/Konami_Justifier) - Lightgun -  Konami Justifier lightgun peripheral (SLEH-00005, SLUH-00017)

- [Mouse](https://en.wikipedia.org/wiki/PlayStation_Mouse) - Mouse - PlayStation Mouse (SCPH-1090, SCPH-1030)

- [neGcon](https://en.wikipedia.org/wiki/NeGcon) - Joypad - Namco third party controller

### User 9 - 16 Device Type(s)

- **RetroPad** - Joypad

### Controllers graph

| Beetle PSX HW  | RetroPad                                                       | PlayStation Controller                                       | DualShock                                                      | Analog Controller                                              | Analog Joystick                                                | neGcon                          |
|----------------|----------------------------------------------------------------|--------------------------------------------------------------|----------------------------------------------------------------|----------------------------------------------------------------|----------------------------------------------------------------|---------------------------------|
| Cross          | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               | ![PS3_Cross](images/Button_Pack/PS3/PS3_Cross.png)           | ![PS3_Cross](images/Button_Pack/PS3/PS3_Cross.png)             | ![PS3_Cross](images/Button_Pack/PS3/PS3_Cross.png)             | ![PS3_Cross](images/Button_Pack/PS3/PS3_Cross.png)             | Analog button I                 |
| Square         | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)               | ![PS3_Square](images/Button_Pack/PS3/PS3_Square.png)         | ![PS3_Square](images/Button_Pack/PS3/PS3_Square.png)           | ![PS3_Square](images/Button_Pack/PS3/PS3_Square.png)           | ![PS3_Square](images/Button_Pack/PS3/PS3_Square.png)           | Analog button II                |
| Select         | ![RetroPad_Select](images/RetroPad/Retro_Select.png)           | ![PS3_Select](images/Button_Pack/PS3/PS3_Select.png)         | ![PS3_Select](images/Button_Pack/PS3/PS3_Select.png)           | ![PS3_Select](images/Button_Pack/PS3/PS3_Select.png)           | ![PS3_Select](images/Button_Pack/PS3/PS3_Select.png)           |                                 |
| Start          | ![RetroPad_Start](images/RetroPad/Retro_Start.png)             | ![PS3_Start](images/Button_Pack/PS3/PS3_Start.png)           | ![PS3_Start](images/Button_Pack/PS3/PS3_Start.png)             | ![PS3_Start](images/Button_Pack/PS3/PS3_Start.png)             | ![PS3_Start](images/Button_Pack/PS3/PS3_Start.png)             | Start                           |
| D-Pad Up       | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            | ![PS3_Dpad_Up](images/Button_Pack/PS3/PS3_Dpad_Up.png)       | ![PS3_Dpad_Up](images/Button_Pack/PS3/PS3_Dpad_Up.png)         | ![PS3_Dpad_Up](images/Button_Pack/PS3/PS3_Dpad_Up.png)         | ![PS3_Dpad_Up](images/Button_Pack/PS3/PS3_Dpad_Up.png)         | D-Pad Up                        |
| D-Pad Down     | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          | ![PS3_Dpad_Down](images/Button_Pack/PS3/PS3_Dpad_Down.png)   | ![PS3_Dpad_Down](images/Button_Pack/PS3/PS3_Dpad_Down.png)     | ![PS3_Dpad_Down](images/Button_Pack/PS3/PS3_Dpad_Down.png)     | ![PS3_Dpad_Down](images/Button_Pack/PS3/PS3_Dpad_Down.png)     | D-Pad Down                      |
| D-Pad Left     | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          | ![PS3_Dpad_Left](images/Button_Pack/PS3/PS3_Dpad_Left.png)   | ![PS3_Dpad_Left](images/Button_Pack/PS3/PS3_Dpad_Left.png)     | ![PS3_Dpad_Left](images/Button_Pack/PS3/PS3_Dpad_Left.png)     | ![PS3_Dpad_Left](images/Button_Pack/PS3/PS3_Dpad_Left.png)     | D-Pad Left                      |
| D-Pad Right    | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         | ![PS3_Dpad_Right](images/Button_Pack/PS3/PS3_Dpad_Right.png) | ![PS3_Dpad_Right](images/Button_Pack/PS3/PS3_Dpad_Right.png)   | ![PS3_Dpad_Right](images/Button_Pack/PS3/PS3_Dpad_Right.png)   | ![PS3_Dpad_Right](images/Button_Pack/PS3/PS3_Dpad_Right.png)   | D-Pad Right                     |
| Circle         | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               | ![PS3_Circle](images/Button_Pack/PS3/PS3_Circle.png)         | ![PS3_Circle](images/Button_Pack/PS3/PS3_Circle.png)           | ![PS3_Circle](images/Button_Pack/PS3/PS3_Circle.png)           | ![PS3_Circle](images/Button_Pack/PS3/PS3_Circle.png)           | A                               |
| Triangle       | ![RetroPad_X](images/RetroPad/Retro_X_Round.png)               | ![PS3_Triangle](images/Button_Pack/PS3/PS3_Triangle.png)     | ![PS3_Triangle](images/Button_Pack/PS3/PS3_Triangle.png)       | ![PS3_Triangle](images/Button_Pack/PS3/PS3_Triangle.png)       | ![PS3_Triangle](images/Button_Pack/PS3/PS3_Triangle.png)       | B                               |
| L1             | ![RetroPad_L1](images/RetroPad/Retro_L1.png)                   | ![PS3_L1](images/Button_Pack/PS3/PS3_L1.png)                 | ![PS3_L1](images/Button_Pack/PS3/PS3_L1.png)                   | ![PS3_L1](images/Button_Pack/PS3/PS3_L1.png)                   | ![PS3_L1](images/Button_Pack/PS3/PS3_L1.png)                   | Left shoulder button (analog)   |
| R1             | ![RetroPad_R1](images/RetroPad/Retro_R1.png)                   | ![PS3_R1](images/Button_Pack/PS3/PS3_R1.png)                 | ![PS3_R1](images/Button_Pack/PS3/PS3_R1.png)                   | ![PS3_R1](images/Button_Pack/PS3/PS3_R1.png)                   | ![PS3_R1](images/Button_Pack/PS3/PS3_R1.png)                   | Right shoulder button (digital) |
| L2             | ![RetroPad_L2](images/RetroPad/Retro_L2.png)                   | ![PS3_L2](images/Button_Pack/PS3/PS3_L2.png)                 | ![PS3_L2](images/Button_Pack/PS3/PS3_L2.png)                   | ![PS3_L2](images/Button_Pack/PS3/PS3_L2.png)                   | ![PS3_L2](images/Button_Pack/PS3/PS3_L2.png)                   | Analog button II                |
| R2             | ![RetroPad_R2](images/RetroPad/Retro_R2.png)                   | ![PS3_R2](images/Button_Pack/PS3/PS3_R2.png)                 | ![PS3_R2](images/Button_Pack/PS3/PS3_R2.png)                   | ![PS3_R2](images/Button_Pack/PS3/PS3_R2.png)                   | ![PS3_R2](images/Button_Pack/PS3/PS3_R2.png)                   | Analog button I                 |
| L3             | ![RetroPad_L3](images/RetroPad/Retro_L3.png)                   |                                                              | ![PS3_L3](images/Button_Pack/PS3/PS3_L3.png)                   |                                                                |                                                                |                                 |
| R3             | ![RetroPad_R3](images/RetroPad/Retro_R3.png)                   |                                                              | ![PS3_R3](images/Button_Pack/PS3/PS3_R3.png)                   |                                                                |                                                                |                                 |
| Left Analog X  | ![RetroPad_Left_Stick](images/RetroPad/Retro_Left_Stick.png)   |                                                              | ![PS3_Left_Stick](images/Button_Pack/PS3/PS3_Left_Stick.png)   | ![PS3_Left_Stick](images/Button_Pack/PS3/PS3_Left_Stick.png)   | Left Joystick X                                                | Twist                           |
| Left Analog Y  | ![RetroPad_Left_Stick](images/RetroPad/Retro_Left_Stick.png)   |                                                              | ![PS3_Left_Stick](images/Button_Pack/PS3/PS3_Left_Stick.png)   | ![PS3_Left_Stick](images/Button_Pack/PS3/PS3_Left_Stick.png)   | Left Joystick Y                                                |                                 |
| Right Analog X | ![RetroPad_Right_Stick](images/RetroPad/Retro_Right_Stick.png) |                                                              | ![PS3_Right_Stick](images/Button_Pack/PS3/PS3_Right_Stick.png) | ![PS3_Right_Stick](images/Button_Pack/PS3/PS3_Right_Stick.png) | Right Joystick X                                               |                                 |
| Right Analog Y | ![RetroPad_Right_Stick](images/RetroPad/Retro_Right_Stick.png) |                                                              | ![PS3_Right_Stick](images/Button_Pack/PS3/PS3_Right_Stick.png) | ![PS3_Right_Stick](images/Button_Pack/PS3/PS3_Right_Stick.png) | Right Joystick Y                                               |                                 |

| RetroMouse                                                      | Guncon / G-Con 45 | Justifier | Mouse        |
|-----------------------------------------------------------------|-------------------|-----------|--------------|
| ![Retro_Mouse](images/RetroMouse/Retro_Mouse.png)               | Pointer           |  Pointer  | Pointer      |
| ![Retro_Left](images/RetroMouse/Retro_Left.png)                 | Trigger†          |  Trigger† | Left button  |
| ![Retro_Middle](images/RetroMouse/Retro_Middle.png)             | B                 |  Start    |              |
| ![Retro_Right](images/RetroMouse/Retro_Right.png)               | A†                |  Aux†     | Right button |
| ![Retro_Left+Middle](images/RetroMouse/Retro_Left+Middle.png)   |                   |           |              |
| ![Retro_Right+Middle](images/RetroMouse/Retro_Right+Middle.png) |                   |           |              |
| Mouse Button 4                                                  | A                 | Aux       |              |
| Mouse Button 5                                                  | B                 | Start     |              |

† These inputs can be modified with the ['Gun Trigger' core option](https://buildbot.libretro.com/docs/library/beetle_psx_hw/#core-options).

**If the 'Gun Trigger' core option is set to Left Mouse Button, then**

- Right click / Mouse Button 4 = Guncon / G-Con 45 'A' and Justifier 'Aux'
- Middle click / Mouse Button 5 = Guncon / G-Con 45 'B' and Justifier 'Start'

**If the 'Gun Trigger' core option is set to  Right Mouse Button, then**

- Left click / Mouse Button 4 = Guncon / G-Con 45 'A' and Justifier 'Aux'
- Middle click / Mouse Button 5 = Guncon / G-Con 45 'B' and Justifier 'Start'

## External Links

- [Beetle PSX HW Libretro Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_psx_hw_libretro.info)
- [Beetle PSX HW Libretro Github Repository](https://github.com/libretro/beetle-psx-libretro)
- [Report Beetle PSX HW Core Issues Here](https://github.com/libretro/beetle-psx-libretro/issues)
- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)