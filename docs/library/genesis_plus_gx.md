# Sega MS/GG/MD/CD (Genesis Plus GX)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/genesis_plus_gx.md). Changes are proposed using "Pull Requests."

## Background

Genesis Plus GX is an open-source Sega 8/16 bit emulator focused on accuracy and portability. The source code, originally based on Genesis Plus 1.3 by Charles MacDonald, has been heavily modified & enhanced, with respect to initial goals and design, in order to improve the accuracy of emulation, implementing new features and adding support for extra peripherals, cartridge & systems hardware.

### Why use this core?

Awaiting description.

### How to get and install the Genesis Plus GX core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Sega MS/GG/MD/CD (Genesis Plus GX)'.

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'Sega MS/GG/MD/CD (Genesis Plus GX)'.

### Authors

- Charles McDonald
- Eke-Eke

## See also

### Sega 16-bit cores

- [Sega Master System (Emux)](https://docs.libretro.com/library/emux_sms/)
- [Sega MS/MD/CD/32X (PicoDrive)](https://docs.libretro.com/library/picodrive/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

- [Non-commercial](https://github.com/libretro/Genesis-Plus-GX/blob/master/LICENSE.txt)

## Extensions

Content that can be loaded by the Genesis Plus GX core have the following file extensions:

- .mdx
- .md
- .smd
- .gen
- .bin
- .cue
- .iso
- .sms
- .gg
- .sg
- .68k
- .chd

## Databases

RetroArch database(s) that are associated with the Genesis Plus GX core:

- [Sega - Game Gear](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Game%20Gear.rdb)
- [Sega - Master System - Mark III](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Master%20System%20-%20Mark%20III.rdb)
- [Sega - Mega-CD - Sega CD](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Mega-CD%20-%20Sega%20CD.rdb)
- [Sega - Mega Drive - Genesis](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Mega%20Drive%20-%20Genesis.rdb)
- [Sega - PICO](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20PICO.rdb)
- [Sega - SG-1000](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20SG-1000.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

|   Filename    |    Description                                  |              md5sum              |
|:-------------:|:-----------------------------------------------:|:--------------------------------:|
| bios_MD.bin   | MegaDrive TMSS startup ROM (bootrom) - Optional | 45e298905a08f9cfb38fd504cd6dbc84 |
| bios_CD_E.bin | MegaCD EU BIOS - Required for MegaCD EU games   | e66fa1dc5820d254611fdcdba0662372 |
| bios_CD_U.bin | SegaCD US BIOS - Required for SegaCD US games   | 854b9150240a198070150e4566ae1290 |
| bios_CD_J.bin | MegaCD JP BIOS - Required for MegaCD JP games   | 278a9397d192149e84e820ac621a8edd |
| bios_E.sms    | MasterSystem EU BIOS (bootrom) - Optional       | -                                |
| bios_U.sms    | MasterSystem US BIOS (bootrom) - Optional       | -                                |
| bios_J.sms    | MasterSystem JP BIOS (bootrom) - Optional       | -                                |
| bios.gg       | GameGear BIOS (bootrom) - Optional              | -                                |
| sk.bin        | Sonic & Knuckles ROM (lock-on) - Optional       | 4ea493ea4e9f6c9ebfccbdb15110367e |
| sk2chip.bin   | Sonic & Knuckles UPMEM ROM (lock-on) - Optional | b4e76e416b887f4e7413ba76fa735f16 |
| areplay.bin   | Action Replay ROM (lock-on) - Optional          | -                                |
| ggenie.bin    | Game Genie ROM (lock-on) - Optional             | -                                |

!!! warning
	BIOS files that are labelled (bootrom) and (lock-on) must have their corresponding [core option](https://docs.libretro.com/library/genesis_plus_gx/#core-options) ('System bootrom' core option or 'Cartridge lock-on' core option) configured correctly in order for them to be loaded.

## Features

RetroArch features that the Genesis Plus GX core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| Core Options      | ✔         |
| RetroAchievements | ✔         |
| RetroArch Cheats  | ✔         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | -         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| Softpatching      | ✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The Genesis Plus GX core's directory name is 'Genesis Plus GX'

The Genesis Plus GX core loads from and saves to to these directories.

**RetroArch's Save directory**

- 'content-name'.srm (MS/GG/MD/Pico/SG-1000 Cartridge Backup save)
- scd_E.brm (Mega CD EU BIOS Backup RAM) **When the 'CD System BRAM' core option is set to per bios**
- scd_U.brm (Sega CD US BIOS Backup RAM) **When the 'CD System BRAM' core option is set to per bios**
- scd_J.brm (Mega CD JP BIOS Backup RAM) **When the 'CD System BRAM' core option is set to per bios**
- 'content-name'.brm (Sega CD/MegaCD Per-game Backup RAM) **When the 'CD System BRAM' core option is set to per game**
- cart.brm (Sega/Mega CD RAM CART)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

The Genesis Plus GX core's internal FPS is (FPS).

The Genesis Plus GX core's internal sample rate is (Rate)

The Genesis Plus GX core's core provided aspect ratio is dependent on the 'Core-provided aspect ratio' [core option](https://docs.libretro.com/library/genesis_plus_gx/#core-options).

### Loading Sega CD games

When loading Sega CD games, Genesis Plus GX needs a cue-sheet that points to an image file. A cue sheet, or cue file, is a metadata file which describes how the tracks of a CD or DVD are laid out.

If you have e.g. `foo.bin`, you should create a text file and save it as `foo.cue`. If the Sega CD game is single-track, the cue file contents should look like this:

`foobin.cue`
```
 FILE "foo.bin" BINARY
  TRACK 01 MODE1/2352
   INDEX 01 00:00:00
```

After that, you can load the `foo.cue` file in RetroArch with the Genesis Plus GX core.

!!! warning ""
    Certain Sega CD games are multi-track, so their .cue files might be more complicated.

## Core options

The Genesis Plus GX core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **System hardware** (**auto**/sg-1000/sg-1000 II/mark-III/master system/master system II/game gear/mega drive / genesis): 

<center> Choose which system is going to be emulated. </center>

- **System region** (**auto**/ntsc-u/pal/ntsc-j): 

<center> Choose which region the system is from. </center>

- **System lockups** (Off/**On**):

<center> Emulate system lockups that occur on real hardware. </center>

- **System bootrom** (**Off**/On):

<center> Runs bootrom if available and then starts loaded content after the boot sequence. Look above at the [BIOS section](https://docs.libretro.com/library/genesis_plus_gx/#bios) for more information. </center>
 
- **CD System BRAM** (**per bios**/per game):

<center> The Sega CD's internal memory cannot hold a lot of saves. Setting this core option to per game allows each game to have its own one brm file, thus negating any lack of available space issues. </center>

- **68k address error** (Off/**On**): 

<center> Emulate the [68k](http://segaretro.org/M68000) address error that occurs on real hardware. Set this to off when playing rom hacks since most emulators used to develop rom hacks don't emulate the error. </center>

- **Cartridge lock-on** (**Off**/game genie/action replay (pro)/sonic & knuckles): 

<center> Select lock-on cartridge. Look above at the [BIOS section](https://docs.libretro.com/library/genesis_plus_gx/#bios) for more information. </center>

- **Master System FM** (**auto**/Off/On):

<center> Enable the Master System FM chip. (Enhanced sound output support for [SMS compatible games](http://segaretro.org/FM_Sound_Unit_).) </center>

- **YM2612 DAC quantization** (**Off**/On): 

<center> for Mame core only. Awaiting description. </center>

- **YM2612/YM3438 core** (**mame**/nuked (ym2612)/nuked (asic ym3438)/nuked (discrete ym3438): 

<center> Awaiting description. </center>

- **Sound output** (**stereo**/mono): 

<center> Self-explanatory. </center>

- **Audio filter** (**Off**/low-pass):

<center> Awaiting description. </center>
 
- **Low-pass filter %** (5 to 95 in increments of 5. **60 is default**): 

<center> Awaiting description. </center>

- **Blargg NTSC filter** (**Off**/monochrome/composite/svidio/rgb):

<center> Self-explanatory. </center>

??? note "*Blargg NTSC filter - Off*"
    ![](images\Cores\genesis_plus_gx\blargg_off.png)

??? note "*Blargg NTSC filter  - monochrome*"
    ![](images\Cores\genesis_plus_gx\blargg_monochrome.png)

??? note "*Blargg NTSC filter - composite*"
    ![](images\Cores\genesis_plus_gx\blargg_composite.png)

??? note "*Blargg NTSC filter  - svideo*"
    ![](images\Cores\genesis_plus_gx\blargg_svideo.png)

??? note "*Blargg NTSC filter - rgb*"
    ![](images\Cores\genesis_plus_gx\blargg_rgb.png)

- **LCD Ghosting filter** (**Off**/On):

<center> Self-explanatory. </center>

??? note "*LCD Ghosting filter - On*"
    ![lcd_ghosting_filter_on](images\Cores\genesis_plus_gx\ghost.png)

- **Borders** (**Off**/ top/bottom/ left/right / full):

<center> Self explanatory. </center>

- **Game Gear extended screen** (**Off**/On):

<center> Self-explanatory. </center>

??? note "*Game Gear extended screen - Off*"
    ![](images\Cores\genesis_plus_gx\extend_off.png)

??? note "*Game Gear extended screen - On*"
    ![](images\Cores\genesis_plus_gx\extend_on.png)

- **Core-provided aspect ratio** (**auto**/NTSC PAR/PAL PAR ): 

<center> Choose the Core-provided aspect ratio. RetroArch's aspect ratio must be set to Core provided in the Video settings for this to function properly. </center>

- **Interlaced mode 2 output** (**single field**/double field):

<center> Change how interlaced mode 2 output is handled. Games like Sonic 2's multiplayer mode uses Interlaced Mode 2. </center>

??? note "*Interlaced mode 2 output - single field*"
    ![interlaced_mode_2_output_single_field](images\Cores\genesis_plus_gx\single.png)
	
??? note "*Interlaced mode 2 output - double field*"
    ![interlaced_mode_2_output_double_field](images\Cores\genesis_plus_gx\double.png)	

- **Show Lightgun crosshair** (**Off**/On):

<center> Shows lightgun crosshairs for the 'MD Menancer', 'MD Justifiers', and 'MS Light Phaser' Device Types. </center>

??? note "*Lightgun crosshair*"
    ![lightgun_crosshair](images\Cores\genesis_plus_gx\lightgun.png)

- **Invert Mouse Y-axis** (**Off**/On):

<center> Inverts the Mouse Y-axis for the 'MD Mouse' Device Type </center>

- **CPU speed** (100% to 200% in increments of 25%. **100% is default**):

<center> Overclock the emulated CPU. </center>

- **Remove per-line sprite limit** (**Off**/On):

<center> Self-explanatory. </center>

## Controllers

### Device types

The Genesis Plus GX core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- Joypad Port Empty - None - Input disabled.
- **Joypad Auto** - Joypad - Depending on the loaded content, the core will automatically emulate a MD Joypad 3 Button controller, or a MD Joypad 6 Button controller or a MS Joypad 2 Button controller
- [MD Joypad 3 Button](https://segaretro.org/Control_Pad_(Mega_Drive)) - Joypad 
- [MD Joypad 6 Button](https://segaretro.org/Six_Button_Control_Pad_(Mega_Drive)) - Joypad
- [MS Joypad 2 Button](https://segaretro.org/Control_Pad_(Master_System)) - Joypad - also used for Game Gear
- [MD Joypad 3 Button + 4-WayPlay](https://segaretro.org/4_Way_Play) - Joypad - Enables multitap
- [MD Joypad 6 Button + 4-WayPlay](https://segaretro.org/4_Way_Play) - Joypad - Enables multitap
- [MD Joypad 3 Button + Teamplayer](https://segaretro.org/Team_Player) - Joypad - Enables multitap
- [MD Joypad 6 Button + Teamplayer](https://segaretro.org/Team_Player) - Joypad - Enables multitap
- MS Joypad 2 Button + Master Tap - Joypad - Enables multitap
- [MS Light Phaser](https://segaretro.org/Light_Phaser) - Lightgun
- [MS Paddle Control](https://segaretro.org/Paddle_Control) - Analog 
- [MS Sports Pad](https://segaretro.org/Sports_Pad) - Analog
- [MS Graphic Board](https://segaretro.org/Sega_Graphic_Board) - Pointer
- [MD XE-1AP](https://segaretro.org/XE-1_AP) - Analog
- [MD Mouse](https://segaretro.org/Sega_Mouse) - Mouse

#### User 2 device types

- Joypad Port Empty - None - Input disabled.
- **Joypad Auto** - Joypad - Depending on the loaded content, the core will automatically emulate a MD Joypad 3 Button controller, or a MD Joypad 6 Button controller or a MS Joypad 2 Button controller
- [MD Joypad 3 Button](https://segaretro.org/Control_Pad_(Mega_Drive)) - Joypad
- [MD Joypad 6 Button](https://segaretro.org/Six_Button_Control_Pad_(Mega_Drive)) - Joypad
- [MS Joypad 2 Button](https://segaretro.org/Control_Pad_(Master_System)) - Joypad - also used for Game Gear
- [MD Joypad 3 Button + 4-WayPlay](https://segaretro.org/4_Way_Play) - Joypad - Enables multitap
- [MD Joypad 6 Button + 4-WayPlay](https://segaretro.org/4_Way_Play) - Joypad - Enables multitap
- [MD Joypad 3 Button + Teamplayer](https://segaretro.org/Team_Player) - Joypad - Enables multitap
- [MD Joypad 6 Button + Teamplayer](https://segaretro.org/Team_Player) - Joypad - Enables multitap
- MS Joypad 2 Button + Master Tap - Joypad - Enables multitap
- [MD Menancer](https://segaretro.org/Menacer) - Lightgun
- [MD Justifiers](https://segaretro.org/The_Justifier)  - Lightgun
- [MS Light Phaser](https://segaretro.org/Light_Phaser) - Lightgun
- [MS Paddle Control](https://segaretro.org/Paddle_Control) - Analog
- [MS Sports Pad](https://segaretro.org/Sports_Pad) - Analog
- [MS Graphic Board](https://segaretro.org/Sega_Graphic_Board) - Pointer
- [MD XE-1AP](https://segaretro.org/XE-1_AP) - Analog
- [MD Mouse](https://segaretro.org/Sega_Mouse) - Mouse

### Other controllers

The Genesis Plus GX can also emulate Pico touch controls but this is done automatically and cannot manually selected as a Device Type through RetroArch's Controls menu.

### Controller tables

#### Joypad and analog device type table

| User 1 - 8 input descriptors  | RetroPad Inputs                              | MD Joypad 3 Button | MD Joypad 6 Button | MS Joypad 2 Button | MS Paddle Control | MS Sports Pad | MD XE-1AP     |
|-------------------------------|----------------------------------------------|--------------------|--------------------|--------------------|-------------------|---------------|---------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                  | B                  | 1                  | 1                 | 1             | E2            |
| A                             | ![](images/RetroPad/Retro_Y_Round.png)       | A                  | A                  |                    |                   |               | E1            |
| Mode                          | ![](images/RetroPad/Retro_Select.png)        |                    | Mode               |                    |                   |               | Select        |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start              | Start              | Start              | Start             | Start         | Start         |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up           | D-Pad Up           | D-Pad Up           |                   |               |               |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down         | D-Pad Down         | D-Pad Down         |                   |               |               |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left         | D-Pad Left         | D-Pad Left         |                   |               |               |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right        | D-Pad Right        | D-Pad Right        |                   |               |               |
| C                             | ![](images/RetroPad/Retro_A_Round.png)       | C                  | C                  | 2                  |                   | 2             |               |
| Y                             | ![](images/RetroPad/Retro_X_Round.png)       |                    | Y                  |                    |                   |               |               |
| X                             | ![](images/RetroPad/Retro_L1.png)            |                    | X                  |                    |                   |               | C             |
| Z                             | ![](images/RetroPad/Retro_R1.png)            |                    | Z                  |                    |                   |               | A             |
| N/A                           | ![](images/RetroPad/Retro_L2.png)            |                    |                    |                    |                   |               | D             |
| N/A                           | ![](images/RetroPad/Retro_R2.png)            |                    |                    |                    |                   |               | B             |
| N/A                           | ![](images/RetroPad/Retro_L3.png)            |                    |                    |                    |                   |               |               |
| N/A                           | ![](images/RetroPad/Retro_R3.png)            |                    |                    |                    |                   |               |               |
| N/A                           | ![](images/RetroPad/Retro_Left_Stick.png) X  |                    |                    |                    | Paddle X          | Trackball X   | Thumb-stick X |
| N/A                           | ![](images/RetroPad/Retro_Left_Stick.png) Y  |                    |                    |                    | Paddle Y          | Trackball Y   | Thumb-stick Y |
| N/A                           | ![](images/RetroPad/Retro_Right_Stick.png) X |                    |                    |                    |                   |               | Slider Y      |
| N/A                           | ![](images/RetroPad/Retro_Right_Stick.png) Y |                    |                    |                    |                   |               | Slider X      |

#### Mouse device type table

| User # input descriptors      | RetroMouse Inputs                        | MD Mouse           | Graphic Board | Pico       |
|-------------------------------|------------------------------------------|--------------------|---------------|------------|
| N/A                           | ![](images/RetroMouse/Retro_Mouse.png)   | Mouse              | Pointer       | Pointer    |
| N/A                           | ![](images/RetroMouse/Retro_Left.png)    | Left button        | Pen           | Pen button |
| N/A                           | ![](images/RetroMouse/Retro_Right.png)   | Right button       | Menu          | Red button |
| N/A                           | Mouse Wheel Down                         | Center button      |               |            |
| N/A                           | ![](images/RetroMouse/Retro_Middle.png)  | Start              | Do            |            |

#### Lightgun device type table

| User # input descriptors      | RetroLightgun Inputs |  MD Menancer       | MD Justifiers | MS Light Phaser |
|-------------------------------|----------------------|--------------------|---------------|-----------------|
| N/A                           | Gun                  | Crosshair          | Crosshair     | Crosshair       |
| N/A                           | Gun Trigger          | A                  | A             | A               |
| N/A                           | Gun Turbo            | B                  | B             | B               |
| N/A                           | Gun Pause            | C                  | C             | C               |
| N/A                           | Gun Start            | Start              | Start         | Start           |

## Compatibility

100% compatibility with Genesis / Mega Drive, Sega/Mega CD, Master System, Game Gear & SG-1000 released software (including all unlicensed or pirate known dumps), also emulating backwards compatibility modes when available. It also has Pico emulation.

## External Links

- [Libretro Genesis Plus GX Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/genesis_plus_gx_libretro.info)
- [Libretro Genesis Plus GX Github Repository](https://github.com/libretro/Genesis-Plus-GX)
- [Report Libretro Genesis Plus GX Core Issues Here](https://github.com/libretro/Genesis-Plus-GX/issues)
- [Official Genesis Plus GX Github Repository](https://github.com/ekeeke/Genesis-Plus-GX)