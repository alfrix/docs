# Sega MS/GG/MD/CD (Genesis Plus GX)

## Background

Genesis Plus GX is an open-source Sega 8/16 bit emulator focused on accuracy and portability. The source code, originally based on Genesis Plus 1.3 by Charles MacDonald, has been heavily modified & enhanced, with respect to initial goals and design, in order to improve the accuracy of emulation, implementing new features and adding support for extra peripherals, cartridge & systems hardware.

### Why use this core?

Awaiting description.

### Authors

- Charles McDonald
- Eke-Eke

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/genesis_plus_gx.md). Changes are proposed using "Pull Requests."

## See also

- [Sega Master System (Emux)](https://doc.libretro.com/library/emux_sms/)
- [Sega MS/GG/MD/CD (Genesis Plus GX)](https://doc.libretro.com/library/genesis_plus_gx/)
- [Sega MS/MD/CD/32X (PicoDrive)](https://doc.libretro.com/library/picodrive/)

## License

- Non-commercial

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

|   Filename    |    Description                         |              md5sum                                                                         |
|:-------------:|:-------------------------------------------------------------------------------------------------:|:--------------------------------:|
| bios_MD.bin   | [MegaDrive TMSS startup ROM (bootrom)](http://segaretro.org/TradeMark_Security_System) - Optional | 45e298905a08f9cfb38fd504cd6dbc84 |
| bios_CD_E.bin | MegaCD EU BIOS - Required for MegaCD EU games                                                     | e66fa1dc5820d254611fdcdba0662372 |
| bios_CD_U.bin | SegaCD US BIOS - Required for SegaCD US games                                                     | 854b9150240a198070150e4566ae1290 |
| bios_CD_J.bin | MegaCD JP BIOS - Required for MegaCD JP games                                                     | 278a9397d192149e84e820ac621a8edd |
| bios_E.sms    | MasterSystem EU BIOS (bootrom) - Optional                                                         | -                                |
| bios_U.sms    | MasterSystem US BIOS (bootrom) - Optional                                                         | -                                |
| bios_J.sms    | MasterSystem JP BIOS (bootrom) - Optional                                                         | -                                |
| bios.gg       | GameGear BIOS (bootrom) - Optional                                                                | -                                |
| sk.bin        | Sonic & Knuckles ROM (lock-on) - Optional                                                         | 4ea493ea4e9f6c9ebfccbdb15110367e |
| sk2chip.bin   | Sonic & Knuckles UPMEM ROM (lock-on) - Optional                                                   | b4e76e416b887f4e7413ba76fa735f16 |
| areplay.bin   | Action Replay ROM (lock-on) - Optional                                                            | -                                |
| ggenie.bin    | Game Genie ROM (lock-on) - Optional                                                               | -                                |

!!! warning
	Firmware files that are labelled (bootrom) and (lock-on) must have their corresponding [core option](https://buildbot.libretro.com/docs/library/genesis_plus_gx/#core-options) ('System bootrom' core option or 'Cartridge lock-on' core option) configured correctly in order for them to be loaded.

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| RetroAchievements | ✔         |
| RetroArch Cheats  | ✔         |
| Native Cheats     | ✕         |
| Controllers       | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | -         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| Softpatching      | -         |

The Genesis Plus GX core's directory name is 'Genesis Plus GX'

- Game data is saved/loaded to and from where save files are stored.
- Save states are saved/loaded to and from where state files are stored.

## Core options

The Genesis Plus GX core has the following options that can be tweaked from the core options menu. The default setting is bolded.

- **System hardware** (**auto**/sg-1000/sg-1000 II/mark-III/master system/master system II/game gear/mega drive / genesis): Choose which system is going to be emulated.
- **System region** (**auto**/ntsc-u/pal/ntsc-j): Choose which region the system is from.
- **System lockups** (Off/**On**): Emulate system lockups that occur on real hardware.
- **System bootrom** (**Off**/On): - Runs bootrom if available and then starts loaded content after the boot sequence. Look above at the [BIOS section](https://buildbot.libretro.com/docs/library/genesis_plus_gx/#bios) for more information.
- **CD System BRAM** (**per bios**/per game): The Sega CD's internal memory cannot hold a lot of saves. Setting this core option to per game allows each game to have its own one brm file, thus negating any lack of available space issues.
- **68k address error** (Off/**On**): Emulate the [68k](http://segaretro.org/M68000) address error that occurs on real hardware. Set this to off when playing rom hacks since most emulators used to develop rom hacks don't emulate the error.
- **Cartridge lock-on** (**Off**/game genie/action replay (pro)/sonic & knuckles): Select lock-on cartridge. Look above at the [BIOS section](https://buildbot.libretro.com/docs/library/genesis_plus_gx/#bios) for more information.
- **Master System FM** (**auto**/Off/On): Enable the Master System FM chip. (Enhanced sound output support for [SMS compatible games](http://segaretro.org/FM_Sound_Unit_).
- **YM2612 DAC quantization** (**Off**/On): Awaiting description.
- **YM2612/YM3438 core** (**mame**/nuked (ym2612)/nuked (asic ym3438)/nuked (discrete ym3438): Awaiting description.
- **Sound output** (**stereo**/mono): Awaiting description.
- **Audio filter** (**Off**/low-pass): - Awaiting description.
- **Low-pass filter %** (5 to 95 in increments of 5. **60 is default**): Awaiting description.
- **Blargg NTSC filter** (**Off**/monochrome/composite/svidio/rgb): Self-explanatory.

??? note "*Blargg NTSC filter - Off*"
    ![blargg_ntsc_filter_disabled](images\Cores\genesis_plus_gx\blargg_ntsc_filter_disabled.png)

??? note "*Blargg NTSC filter  - monochrome*"
    ![blargg_ntsc_filter_monochrome](images\Cores\genesis_plus_gx\blargg_ntsc_filter_monochrome.png)

??? note "*Blargg NTSC filter - composite*"
    ![blargg_ntsc_filter_composite](images\Cores\genesis_plus_gx\blargg_ntsc_filter_composite.png)

??? note "*Blargg NTSC filter  - svideo*"
    ![blargg_ntsc_filter_svideo](images\Cores\genesis_plus_gx\blargg_ntsc_filter_svideo.png)

??? note "*Blargg NTSC filter - rgb*"
    ![blargg_ntsc_filter_rgb](images\Cores\genesis_plus_gx\blargg_ntsc_filter_rgb.png)

- **LCD Ghosting filter** (**Off**/On): Self-explanatory.

??? note "*LCD Ghosting filter - On*"
    ![lcd_ghosting_filter_on](images\Cores\genesis_plus_gx\lcd_ghosting_filter_on.png)

- **Borders** (**Off**/ top/bottom/ left/right / full): Self explanatory.
- **Game Gear extended screen** (**Off**/On): Self-explanatory.

??? note "*Game Gear extended screen - Off*"
    ![game_gear_extended_screen_off](images\Cores\genesis_plus_gx\game_gear_extended_screen_off.png)

??? note "*Game Gear extended screen - On*"
    ![game_gear_extended_screen_on](images\Cores\genesis_plus_gx\game_gear_extended_screen_on.png)

- **Core-provided aspect ratio** (**auto**/NTSC PAR/PAL PAR ): Choose the Core-provided aspect ratio. RetroArch's aspect ratio must be set to Core provided in the Video settings for this to function properly.

- **Interlaced mode 2 output** (**single field**/double field): Change how interlaced mode 2 output is handled. Games like Sonic 2's multiplayer mode uses Interlaced Mode 2.

??? note "*Interlaced mode 2 output - single field*"
    ![interlaced_mode_2_output_single_field](images\Cores\genesis_plus_gx\interlaced_mode_2_output_single_field.png)
	
??? note "*Interlaced mode 2 output - double field*"
    ![interlaced_mode_2_output_double_field](images\Cores\genesis_plus_gx\interlaced_mode_2_output_double_field.png)	

- **Show Lightgun crosshair** (**Off**/On): Shows lightgun crosshairs for the 'MD Menancer', 'MD Justifiers', and 'MS Light Phaser' Device Types.

??? note "*Lightgun crosshair*"
    ![lightgun_crosshair](images\Cores\genesis_plus_gx\lightgun_crosshair.png)

- **Invert Mouse Y-axis** (**Off**/On): Inverts the Mouse Y-axis for the 'MD Mouse' Device Type

- **CPU speed** (100% to 200% in increments of 25%. **100% is default**): Overclock the emulated CPU.

- **Remove per-line sprite limit** (**Off**/On): Self-explanatory.

## Controllers

The Genesis Plus GX core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):

### User 1 Device Type(s)

- **Joypad Auto** - Joypad - Depending on the loaded content, the core will automatically emulate a MD Joypad 3 Button controller, or a MD Joypad 6 Button controller or a MS Joypad 2 Button controller

- MD Joypad 3 Button - Joypad 

- MD Joypad 6 Button - Joypad

- MS Joypad 2 Button - Joypad - also used for Game Gear

- MD Joypad 3 Button + 4-WayPlay - Joypad - allows for up to four players to play together in certain games

- MD Joypad 6 Button + 4-WayPlay - Joypad - allows for up to four players to play together in certain games

- MD Joypad 3 Button + Teamplayer - Joypad - allows for up to four players to play together in certain games

- MD Joypad 6 Button + Teamplayer - Joypad - allows for up to four players to play together in certain games

- MS Joypad 2 Button + Master Tap - Joypad - allows for up to four players to play together in certain games

- MS Light Phaser - Lightgun

- MS Paddle Control - Joypad 

- MS Sports Pad - Joypad

- MS Graphic Board - Pointer

- MD XE-1AP - Joypad

- MD Mouse - Mouse

### User 2 Device Type(s)

- **Joypad Auto** - Joypad - Depending on the loaded content, the core will automatically emulate a MD Joypad 3 Button controller, or a MD Joypad 6 Button controller or a MS Joypad 2 Button controller

- MD Joypad 3 Button - Joypad

- MD Joypad 6 Button - Joypad

- MS Joypad 2 Button - Joypad - also used for Game Gear

- MD Joypad 3 Button + 4-WayPlay - Joypad - allows for up to four players to play together in certain games

- MD Joypad 6 Button + 4-WayPlay - Joypad - allows for up to four players to play together in certain games

- MD Joypad 3 Button + Teamplayer - Joypad - allows for up to four players to play together in certain games

- MD Joypad 6 Button + Teamplayer - Joypad - allows for up to four players to play together in certain games

- MS Joypad 2 Button + Master Tap - Joypad - allows for up to four players to play together in certain games

- MD Menancer - Lightgun

- MD Justifiers  - Lightgun

- MS Light Phaser - Lightgun

- MS Paddle Control - Joypad

- MS Sports Pad - Joypad

- MS Graphic Board - Pointer

- MD XE-1AP - Joypad

- MD Mouse - Mouse

### User 3 - 16 Device Type(s)

- **RetroPad** - Joypad

### Controllers graph

| Genesis Plus GX  | RetroPad                                                       |  MD Joypad 3 Button (+ 4-WayPlay) (+ Teamplayer)  |  MD Joypad 6 Button (+ 4-WayPlay) (+ Teamplayer)  |  MS Joypad 2 Button (+ Master Tap)  |  MS Paddle Control  |  MS Sports Pad  |  MD XE-1AP  |
|------------------|----------------------------------------------------------------|---------------------------------------------------|---------------------------------------------------|-------------------------------------|---------------------|-----------------|-------------|
| B                | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               | B                                                 | B                                                 | 1                                   | 1                   | 1               | E2          |
| A                | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)               | A                                                 | A                                                 |                                     |                     |                 | E1          |
| Mode             | ![RetroPad_Select](images/RetroPad/Retro_Select.png)           |                                                   | Mode                                              |                                     |                     |                 | Select      |
| Start            | ![RetroPad_Start](images/RetroPad/Retro_Start.png)             | Start                                             | Start                                             | Start                               | Start               | Start           | Start       |
| D-pad            | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad.png)               | D-pad                                             | D-pad                                             | D-pad                               |                     |                 |             |
| C                | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               | C                                                 | C                                                 | 2                                   |                     | 2               |             |
| Y                | ![RetroPad_X](images/RetroPad/Retro_X_Round.png)               |                                                   | Y                                                 |                                     |                     |                 |             |
| X                | ![RetroPad_L1](images/RetroPad/Retro_L1.png)                   |                                                   | X                                                 |                                     |                     |                 | C           |
| Y                | ![RetroPad_R1](images/RetroPad/Retro_R1.png)                   |                                                   | Z                                                 |                                     |                     |                 | A           |
|                  | ![RetroPad_L2](images/RetroPad/Retro_L2_Temp.png)              |                                                   |                                                   |                                     |                     |                 | D           |
|                  | ![RetroPad_R2](images/RetroPad/Retro_R2.png)                   |                                                   |                                                   |                                     |                     |                 | B           |
|                  | ![RetroPad_Left_Stick](images/RetroPad/Retro_Left_Stick.png)   |                                                   |                                                   |                                     | Paddle              | Trackball       | Thumb-stick |
|                  | ![RetroPad_Right_Stick](images/RetroPad/Retro_Right_Stick.png) |                                                   |                                                   |                                     |                     |                 | Slider      |

| RetroMouse                                                      |  Menacer  |  Justifiers  |  Light Phaser  |  Graphic Board  |  MD Mouse  |
|-----------------------------------------------------------------|-----------|--------------|----------------|-----------------|------------|
| ![Retro_Mouse](images/RetroMouse/Retro_Mouse.png)               | Pointer   | Pointer      | Pointer        | Pointer         | Pointer    | 
| ![RetroP_Left](images/RetroMouse/Retro_Left.png)                | A         | A            | A              | Pen             | Left       |
| Mouse wheel down                                                |           |              |                |                 | Center     |
| ![Retro_Middle](images/RetroMouse/Retro_Middle.png)             |           |              |                | Do              | Start      |
| ![Retro_Right](images/RetroMouse/Retro_Right.png)               | B         | B            | B              | Menu            | Right      |
| ![Retro_Left+Middle](images/RetroMouse/Retro_Left+Middle.png)   | C         | C            | C              |                 |            |
| ![Retro_Right+Middle](images/RetroMouse/Retro_Right+Middle.png) | Start     | Start        | Start          |                 |            |

## Compatibility

100% compatibility with Genesis / Mega Drive, Sega/Mega CD, Master System, Game Gear & SG-1000 released software (including all unlicensed or pirate known dumps), also emulating backwards compatibility modes when available.

## External Links

- [Libretro Genesis Plus GX Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/genesis_plus_gx_libretro.info)
- [Libretro Genesis Plus GX Github Repository](https://github.com/libretro/Genesis-Plus-GX)
- [Report Libretro Genesis Plus GX Core Issues Here](https://github.com/libretro/Genesis-Plus-GX/issues)
- [Official Genesis Plus GX Github Repository](https://github.com/ekeeke/Genesis-Plus-GX)