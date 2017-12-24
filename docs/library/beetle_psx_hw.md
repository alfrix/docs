# PlayStation (Beetle PSX HW)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_psx_hw.md). Changes are proposed using "Pull Requests."

There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)

You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).

## Background

Enhanced port of standalone Mednafen PSX to libretro.

### Why use this core?

Awaiting description.

### How to get and install the Beetle PSX HW core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'PlayStation (Beetle PSX HW)'.

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'PlayStation (Beetle PSX HW)'.

The content should now start running!

### Authors

- [Mednafen Team](https://mednafen.github.io/)

## See also

### PSX

- [PlayStation (Beetle PSX)](https://docs.libretro.com/library/beetle_psx/)
- [PlayStation (PCSX ReARMed)](https://docs.libretro.com/library/pcsx_rearmed/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Beetle PSX HW core is licensed under

- [GPLv2](https://github.com/libretro/beetle-psx-libretro/blob/master/COPYING)

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

RetroArch-level settings or features that the Beetle PSX HW core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| Core Options      | ✔         |
| RetroAchievements | ✕         |
| RetroArch Cheats  | ✔         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | -         |
| Rumble            | ✔         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| Softpatching      | ✕         |
| Disk Control      | ✔         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The Beetle PSX HW core's directory name is 'Beetle PSX HW'

The Beetle PSX HW core saves/loads to/from these directories.

**RetroArch's Save directory**

- Memory cards

**RetroArch's State directory**

- 'content-name'.srm (State)

### Geometry and timing

- The Beetle PSX HW core's internal FPS is (FPS)
- The Beetle PSX HW core's internal sample rate is (Rate)
- The Beetle PSX HW core's core provided aspect ratio is (Ratio)

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

!!! attention
    Certain PS1 games are multi-track, so their .cue files might be more complicated.
	
#### Playing PAL copy protected games

PAL copy protected games need a SBI Subchannel file next to the bin/cue files in order to get past the copy protection.

- Ape Escape (Europe).bin
- Ape Escape (Europe).cue
- **Ape Escape (Europe).sbi**

!!! warning
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

![](images\Cores\beetle_psx_hw\m3u.png)

!!! attention
	Adding multi-track games to a RetroArch playlist is recommended. (Manually add an entry a playlist that points to `foo.m3u`)

### Game compression

Alternatively to using cue sheets with .bin files, you can convert your games to .pbp (Playstation Portable update file) to reduce file sizes and neaten up your game folder. A recommended .pbp convert tool is PSX2PSP.

If converting a multiple-disk game, all disks should be added to the same .pbp file, rather than making a .m3u file for them.

Most conversion tools will want a single .bin file for each disk. If your game uses multiple .bin files (tracks) per disk, you will have to mount the cue sheet to a virtual drive and re-burn the images onto a single track before conversion.

!!! attention
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

!!! attention
    Memory card behavior can be controlled with the following [core options](https://docs.libretro.com/library/beetle_psx/#core-options) (Memcard 0 method, Enable memory card 1, Shared memcards).

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

!!! attention
	To import your old memory cards from other emulators, you need to rename them to either the Libretro savedata format or the Mednafen savedata format.

!!! warning
	Keep in mind that save states also include the state of the memory card; carelessly loading an old save state will **OVEWRITE** the memory card, potentially resulting in lost saved games. **You can set the 'Don't overwrite SaveRAM on loading savestate' option in RetroArch's Saving settings to On to prevent this.**

## Core options

*The Beetle PSX HW core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.*

- **Renderer (restart)** (**vulkan**/opengl/software)

<center> Choose which video renderer will be used. **Software is the most accurate renderer.** The OpenGL and Vulkan renderers will enable and/or speedup enhancements like upscaling and texture filtering. **The OpenGL and Vulkan renderers must be used with its corresponding video driver in RetroArch's Driver settings.** **Also, Hardware Shared Context must be enabled in RetroArch's Core settings.** </center>

- **Software framebuffer** (Off/**On**)

<center> If off, the software renderer will skip some steps. Potential speedup. Causes bad graphics when doing framebuffer readbacks.

- **Adaptive smoothing** (Off/**On**)

<center> When upscaling, smooths out 2D elements while keeping 3D elements sharp. Only for the Vulkan renderer at the moment. </center>

??? note "*Adapative smoothing - Off*"
    ![](images\Cores\beetle_psx_hw\smooth_off.png)

??? note "*Adaptive smoothing - On*"
    ![](images\Cores\beetle_psx_hw\smooth_on.png)

- **Internal GPU resolution** (**1x(native)**/2x/4x/8x/16x/32x)

<center> Modify the resolution. </center>

??? note "*Internal GPU Resolution - 1x*"
    ![](images\Cores\beetle_psx_hw\gpu_1.png)

??? note "*Internal GPU Resolution - 2x*"
    ![](images\Cores\beetle_psx_hw\gpu_2.png)

- **Texture filtering** (**nearest**/SABR/xBR/bilinear/3-point/JINC2)

<center> Per-texture filtering. Only for the OpenGL renderer at the moment. </center>

??? note "*nearest*"
    ![](images\Cores\beetle_psx_hw\nearest.png)

??? note "*SABR*"
    ![](images\Cores\beetle_psx_hw\sabr.png)

??? note "*xBR*"
    ![](images\Cores\beetle_psx_hw\xbr.png)

??? note "*bilinear*"
    ![](images\Cores\beetle_psx_hw\bilinear.png)

??? note "*3-point*"
    ![](images\Cores\beetle_psx_hw\3point.png)

??? note "*JINC2*"
    ![](images\Cores\beetle_psx_hw\jinc2.png)

- **Internal color depth** (**dithered 16bpp (native)**/32bpp)

<center> PSX had 16bpp depth, Beetle PSX HW can go up to 32bpp. **Only for the OpenGL and Vulkan renderers at the moment.** The Vulkan renderer always uses 32bpp. </center>

- **Wireframe mode** (**Off**/On)

<center> Shows only the outlines of polygons. Only for the OpenGL renderer. **For debug use.** </center>

??? note "Wireframe mode - On"
	![](images\Cores\beetle_psx_hw\wire.png)

- **Display full VRAM** (**Off**/On)

<center> Everything in VRAM is drawn on screen. **For debug use.** </center>

??? note "Display full VRAM - On"
	![](images\Cores\beetle_psx_hw\vram.png)

- **PGXP operation mode** (**Off**/memory only/memory + CPU)

<center> When on, floating point coordinates will be used for vertex positions, to avoid the PSX polygon jitter. 'memory + cpu' mode can further reduce jitter at the cost of performance and geometry glitches. </center>

- **PGXP vertex cache** (**Off**/On)

<center> Maintains a cache for vertices. May result in better performance but can result in graphics glitches in most games. </center>

- **PGXP perspective correct texturing** (**Off**/On)

<center> Original PSX did affine texture mapping, resulting in e.g. crooked lines across walls. This fixes it. </center>

- **Widescreen mode hack** (**Off**/On)

<center> If on, renders in 16:9. Works best on 3D games. </center>

??? note "Widescreen mode hack - Off"
	![](images\Cores\beetle_psx_hw\wide_off.png)
	
??? note "Widescreen mode hack - On"
	![](images\Cores\beetle_psx_hw\wide_on.png)

- **Frame duping (speedup)** (**Off**/On)

<center> Redraws/reuses the last frame if there was no new data. </center>

- **CPU Overclock** (**Off**/On)

Gets rid of memory access latency and makes all GTE instructions have 1 cycle latency. </center>

- **Skip BIOS** (**Off**/On)

<center> Self-explanatory. **Some games have issues when this core option is enabled (Saga Frontier, PAL copy protected games, etc).** </center>

??? note "Skip BIOS - Off"
	![](images\Cores\beetle_psx_hw\bios.png)

- **Dithering pattern** (**1x(native)**/internal resolution/Off): 

<center> If off, disables the dithering pattern the PSX applies to combat color banding. **Only for the OpenGL and Software renderers. Vulkan always disables the pattern.** </center>

- **Display internal FPS** (**Off**/On)

<center> Shows the frame rate at which the emulated PSX is drawing at. **Onscreen Notifications must be enabled in the RetroArch Onscreen Display Settings.** </center>

??? note "Display internal FPS - On"
	![](images\Cores\beetle_psx_hw\fps.png)

- **Initial scanline** (0 to 40 in increments of 1. **0 is default**)

<center> Sets the first scanline to be drawn on screen. </center>

- **Last scanline** (210 to 239 in increments of 1. **239 is default**)

<center> Sets the last scanline to be drawn on screen. </center>

- **Initial scanline PAL** (0 to 40 in increments of 1. **0 is default**)

<center> Sets the first scanline to be drawn on screen for PAL systems. </center>

- **Last scanline PAL** (260 to 287 in increments of 1. **287 is default**)

<center> Sets the last scanline to be drawn on screen for PAL systems. </center>

- **Crop Overscan** (Off/**On**)

<center> Crop out the potentially random glitchy video output that would have been hidden by the bezel around the edge of a standard-definition television screen. </center>

??? note "Crop Overscan - On"
	![](images\Cores\beetle_psx_hw\scan_on.png)
	
??? note "Crop Overscan - Off"
	![](images\Cores\beetle_psx_hw\scan_on.png)

- **Additional Cropping** (**Off**/1 px/2 px/3 px/4 px/5 px/6 px/7 px/8 px)

<center> Self-explanatory. </center>

- **Offset Cropped Image** (**Off**/1 px/2 px/3 px/4 px/-4 px/-3 px/-2 px/-1 px)

<center> Self-explanatory. </center>

- **Analog self-calibration** (**Off**/On)

<center> When enabled, monitors the max values reached by the input, using it as a calibration heuristic which then scales the analog coordinates sent to the emulator accordingly. For best results, rotate the sticks at max amplitude for the algorithm to get a good estimate of the scaling factor, otherwise it will adjust while playing. </center>

- **DualShock Analog button toggle** (**Off**/On)

<center> Toggles the Analog button from DualShock controllers, if disabled analogs are always on, if enabled you can toggle their state by pressing and holding START+SELECT+L1+L2+R1+R2. </center>

- **Port 1: Multitap enable** (**Off**/On)

<center> Enables/Disables multitap functionality on port 1. </center>

- **Port 2: Multitap enable** (**Off**/On)

<center> Enables/Disables multitap functionality on port 2. </center>

- **Gun Cursor** (**Cross**/Dot/Off)

<center> Choose the cursor for the 'Guncon / G-Con 45' and 'Justifier' Device Types. Setting it to off disables the crosshair. </center>

??? note "Gun Cursor - Cross"
	![](images\Cores\beetle_psx_hw\cursor_cross.png)
	
??? note "Gun Cursor - Dot"
	![](images\Cores\beetle_psx_hw\cursor_dot.png)	

??? note "Gun Cursor - Off"
	![](images\Cores\beetle_psx_hw\cursor_off.png)		
	
- **Mouse Sensitivity** (5% to 200% in increments of 5%. **100% is default**)

<center> Configure the 'Mouse' Device Type's sensitivity. </center>

- **CD Access Method (restart)** (**sync**/async/precache)

<center> The precache setting loads the complete image in memory at startup. Can potentially decrease loading times at the cost of increased startup time. </center>

- **Memcard 0 method** (**libretro**/mednafen)

<center> Choose the savedata format used for Memcard 0 (libretro or mednafen). Look above at the [Saves section](https://docs.libretro.com/library/beetle_psx_hw/#saves) for an explanation regarding the libretro and mednafen formats. <center>

- **Enable memory card 1** (Off/**On**)

<centeR> Enable or disables Memcard slot 1. When disabled, games cannot save/load to Memcard slot 1.  **Memcard 1 must be enabled for game 'Codename Tenka'.** </center>

- **Shared memcards (restart)** (**Off**/On)

<center> Games will share and save/load to the same memory cards. </center>

<center>

| Memcard slot 0                     | Memcard slot 1                     |
|------------------------------------|------------------------------------|
| mednafen_psx_libretro_shared.0.mcr | mednafen_psx_libretro_shared.1.mcr |

</center>

!!! attention
	The 'Memcard 0 method' core option needs to be set to 'mednafen' for the 'Shared memcards' core option to function properly.

- **Increase CD loading speed** (**2x (native)**/4x/6x/8x/10x/12x/14x)

<center> An **experimental** feature, may not work correctly in all games. Some games may break if you set them past a certain speed. Can greatly reduce the loading times on games. </center>

## Controllers

### Device types

The Beetle PSX HW core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 8 device types

- None - Input disabled.
- [**PlayStation Controller**](https://en.wikipedia.org/wiki/PlayStation_Controller) - Joypad - PlayStation Controller (SCPH-1080)
- [DualShock](https://en.wikipedia.org/wiki/DualShock) - Joypad - DualShock (SCPH-1200)
- [Analog Controller](https://en.wikipedia.org/wiki/Dual_Analog_Controller) - Joypad - PlayStation Dual Analog Controller(SCPH-1180)
- [Analog Joystick](https://en.wikipedia.org/wiki/PlayStation_Analog_Joystick) - Joypad - PlayStation Analog Joystick (SCPH-1110)
- [Guncon / G-Con 45](https://en.wikipedia.org/wiki/GunCon) - Lightgun - Namco Gun Controller (SLEH-00007)
- [Justifier](https://en.wikipedia.org/wiki/Konami_Justifier) - Lightgun -  Konami Justifier lightgun peripheral (SLEH-00005, SLUH-00017)
- [Mouse](https://en.wikipedia.org/wiki/PlayStation_Mouse) - Mouse - PlayStation Mouse (SCPH-1090, SCPH-1030)
- [neGcon](https://en.wikipedia.org/wiki/NeGcon) - Joypad - Namco third party controller

### Rumble support

Rumble only works in the Beetle PSX HW core when

- The content being ran has rumble support.
- The joypad input driver being used has rumble support. (e.g. Xinput)
- The joypad device being used has rumble support.
- The corresponding user's device type is set to **DualShock**

### Multitap support

['Port 1: Multitap enable' and 'Port 2: Multitap enable' core options](https://docs.libretro.com/library/beetle_psx_hw#core-options).

### Controller tables

#### Joypad and analog device type table

| User 1 - 8 Input descriptors  | RetroPad Inputs                                                | PlayStation Controller                                       | DualShock                                                      | Analog Controller                                              | Analog Joystick                                                | neGcon                          |
|-------------------------------|----------------------------------------------------------------|--------------------------------------------------------------|----------------------------------------------------------------|----------------------------------------------------------------|----------------------------------------------------------------|---------------------------------|
| Cross                         | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               | ![PS3_Cross](images/Button_Pack/PS3/PS3_Cross.png)           | ![PS3_Cross](images/Button_Pack/PS3/PS3_Cross.png)             | ![PS3_Cross](images/Button_Pack/PS3/PS3_Cross.png)             | ![PS3_Cross](images/Button_Pack/PS3/PS3_Cross.png)             | Analog button I                 |
| Square                        | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)               | ![PS3_Square](images/Button_Pack/PS3/PS3_Square.png)         | ![PS3_Square](images/Button_Pack/PS3/PS3_Square.png)           | ![PS3_Square](images/Button_Pack/PS3/PS3_Square.png)           | ![PS3_Square](images/Button_Pack/PS3/PS3_Square.png)           | Analog button II                |
| Select                        | ![RetroPad_Select](images/RetroPad/Retro_Select.png)           | ![PS3_Select](images/Button_Pack/PS3/PS3_Select.png)         | ![PS3_Select](images/Button_Pack/PS3/PS3_Select.png)           | ![PS3_Select](images/Button_Pack/PS3/PS3_Select.png)           | ![PS3_Select](images/Button_Pack/PS3/PS3_Select.png)           |                                 |
| Start                         | ![RetroPad_Start](images/RetroPad/Retro_Start.png)             | ![PS3_Start](images/Button_Pack/PS3/PS3_Start.png)           | ![PS3_Start](images/Button_Pack/PS3/PS3_Start.png)             | ![PS3_Start](images/Button_Pack/PS3/PS3_Start.png)             | ![PS3_Start](images/Button_Pack/PS3/PS3_Start.png)             | Start                           |
| D-Pad Up                      | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            | ![PS3_Dpad_Up](images/Button_Pack/PS3/PS3_Dpad_Up.png)       | ![PS3_Dpad_Up](images/Button_Pack/PS3/PS3_Dpad_Up.png)         | ![PS3_Dpad_Up](images/Button_Pack/PS3/PS3_Dpad_Up.png)         | ![PS3_Dpad_Up](images/Button_Pack/PS3/PS3_Dpad_Up.png)         | D-Pad Up                        |
| D-Pad Down                    | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          | ![PS3_Dpad_Down](images/Button_Pack/PS3/PS3_Dpad_Down.png)   | ![PS3_Dpad_Down](images/Button_Pack/PS3/PS3_Dpad_Down.png)     | ![PS3_Dpad_Down](images/Button_Pack/PS3/PS3_Dpad_Down.png)     | ![PS3_Dpad_Down](images/Button_Pack/PS3/PS3_Dpad_Down.png)     | D-Pad Down                      |
| D-Pad Left                    | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          | ![PS3_Dpad_Left](images/Button_Pack/PS3/PS3_Dpad_Left.png)   | ![PS3_Dpad_Left](images/Button_Pack/PS3/PS3_Dpad_Left.png)     | ![PS3_Dpad_Left](images/Button_Pack/PS3/PS3_Dpad_Left.png)     | ![PS3_Dpad_Left](images/Button_Pack/PS3/PS3_Dpad_Left.png)     | D-Pad Left                      |
| D-Pad Right                   | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         | ![PS3_Dpad_Right](images/Button_Pack/PS3/PS3_Dpad_Right.png) | ![PS3_Dpad_Right](images/Button_Pack/PS3/PS3_Dpad_Right.png)   | ![PS3_Dpad_Right](images/Button_Pack/PS3/PS3_Dpad_Right.png)   | ![PS3_Dpad_Right](images/Button_Pack/PS3/PS3_Dpad_Right.png)   | D-Pad Right                     |
| Circle                        | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               | ![PS3_Circle](images/Button_Pack/PS3/PS3_Circle.png)         | ![PS3_Circle](images/Button_Pack/PS3/PS3_Circle.png)           | ![PS3_Circle](images/Button_Pack/PS3/PS3_Circle.png)           | ![PS3_Circle](images/Button_Pack/PS3/PS3_Circle.png)           | A                               |
| Triangle                      | ![RetroPad_X](images/RetroPad/Retro_X_Round.png)               | ![PS3_Triangle](images/Button_Pack/PS3/PS3_Triangle.png)     | ![PS3_Triangle](images/Button_Pack/PS3/PS3_Triangle.png)       | ![PS3_Triangle](images/Button_Pack/PS3/PS3_Triangle.png)       | ![PS3_Triangle](images/Button_Pack/PS3/PS3_Triangle.png)       | B                               |
| L1                            | ![RetroPad_L1](images/RetroPad/Retro_L1.png)                   | ![PS3_L1](images/Button_Pack/PS3/PS3_L1.png)                 | ![PS3_L1](images/Button_Pack/PS3/PS3_L1.png)                   | ![PS3_L1](images/Button_Pack/PS3/PS3_L1.png)                   | ![PS3_L1](images/Button_Pack/PS3/PS3_L1.png)                   | Left shoulder button (analog)   |
| R1                            | ![RetroPad_R1](images/RetroPad/Retro_R1.png)                   | ![PS3_R1](images/Button_Pack/PS3/PS3_R1.png)                 | ![PS3_R1](images/Button_Pack/PS3/PS3_R1.png)                   | ![PS3_R1](images/Button_Pack/PS3/PS3_R1.png)                   | ![PS3_R1](images/Button_Pack/PS3/PS3_R1.png)                   | Right shoulder button (digital) |
| L2                            | ![RetroPad_L2](images/RetroPad/Retro_L2.png)                   | ![PS3_L2](images/Button_Pack/PS3/PS3_L2.png)                 | ![PS3_L2](images/Button_Pack/PS3/PS3_L2.png)                   | ![PS3_L2](images/Button_Pack/PS3/PS3_L2.png)                   | ![PS3_L2](images/Button_Pack/PS3/PS3_L2.png)                   | Analog button II                |
| R2                            | ![RetroPad_R2](images/RetroPad/Retro_R2.png)                   | ![PS3_R2](images/Button_Pack/PS3/PS3_R2.png)                 | ![PS3_R2](images/Button_Pack/PS3/PS3_R2.png)                   | ![PS3_R2](images/Button_Pack/PS3/PS3_R2.png)                   | ![PS3_R2](images/Button_Pack/PS3/PS3_R2.png)                   | Analog button I                 |
| L3                            | ![RetroPad_L3](images/RetroPad/Retro_L3.png)                   |                                                              | ![PS3_L3](images/Button_Pack/PS3/PS3_L3.png)                   |                                                                |                                                                |                                 |
| R3                            | ![RetroPad_R3](images/RetroPad/Retro_R3.png)                   |                                                              | ![PS3_R3](images/Button_Pack/PS3/PS3_R3.png)                   |                                                                |                                                                |                                 |
| Left Analog X                 | ![RetroPad_Left_Stick](images/RetroPad/Retro_Left_Stick.png)   |                                                              | ![PS3_Left_Stick](images/Button_Pack/PS3/PS3_Left_Stick.png)   | ![PS3_Left_Stick](images/Button_Pack/PS3/PS3_Left_Stick.png)   | Left Joystick X                                                | Twist                           |
| Left Analog Y                 | ![RetroPad_Left_Stick](images/RetroPad/Retro_Left_Stick.png)   |                                                              | ![PS3_Left_Stick](images/Button_Pack/PS3/PS3_Left_Stick.png)   | ![PS3_Left_Stick](images/Button_Pack/PS3/PS3_Left_Stick.png)   | Left Joystick Y                                                |                                 |
| Right Analog X                | ![RetroPad_Right_Stick](images/RetroPad/Retro_Right_Stick.png) |                                                              | ![PS3_Right_Stick](images/Button_Pack/PS3/PS3_Right_Stick.png) | ![PS3_Right_Stick](images/Button_Pack/PS3/PS3_Right_Stick.png) | Right Joystick X                                               |                                 |
| Right Analog Y                | ![RetroPad_Right_Stick](images/RetroPad/Retro_Right_Stick.png) |                                                              | ![PS3_Right_Stick](images/Button_Pack/PS3/PS3_Right_Stick.png) | ![PS3_Right_Stick](images/Button_Pack/PS3/PS3_Right_Stick.png) | Right Joystick Y                                               |                                 |

#### Mouse device type table

| User 1 - 8 Input descriptors  | RetroMouse Inputs                        | Mouse              |
|-------------------------------|------------------------------------------|--------------------|
|                               | ![](images/RetroMouse/Retro_Mouse.png)   | Mouse pointer      |
|                               | ![](images/RetroMouse/Retro_Left.png)    | Left buttpn        |
|                               | ![](images/RetroMouse/Retro_Right.png)   | Right button       |

#### Lightgun device type table

| User 1 - 8 Input descriptors  | RetroLightgun Inputs | Guncon / G-Con 45         | Justifier         |
|-------------------------------|----------------------|---------------------------|-------------------|
|                               | Gun                  | Guncon / G-Con 45 pointer | Justifier pointer |
|                               | Gun Trigger          | Trigger                   | Trigger           |
|                               | Gun Reload           | Reload                    | Reload            |
|                               | Gun Aux A            | A                         | Aux               |
|                               | Gun Aux B            | B                         |                   |
|                               | Gun Start            |                           | Start             |

## Compatibility

Awaiting description.

## External Links

- [Beetle PSX HW Libretro Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_psx_hw_libretro.info)
- [Beetle PSX HW Libretro Github Repository](https://github.com/libretro/beetle-psx-libretro)
- [Report Beetle PSX HW Core Issues Here](https://github.com/libretro/beetle-psx-libretro/issues)
- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)