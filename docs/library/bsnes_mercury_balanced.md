# SNES / Super Famicom (bsnes-mercury Balanced)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/bsnes_mercury_balanced.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

bsnes-mercury is a fork of higan, aiming to restore some useful features that have been removed, as well as improving performance a bit.
Maximum accuracy is still uncompromisable; anything that affects accuracy is optional and off by default.

This core has been compiled with the Balanced profile.

### Why use this core?

Improvements include:

* Improved framerate
* Faster ROM loading
* HLE emulation of some special chips is optionally restored (defaults to LLE), to improve performance and reduce reliance on those chip ROMs (they're not really easy to find). Chips for which no HLE emulation was developed (ST-0011 and ST-0018) are still LLE.
* SuperFX overclock is now available (off by default, of course); if enabled, it makes SuperFX look quite a lot smoother.

**The bsnes-mercury cores are not less accurate at default settings than the mainline bsnes cores (you have to explicitly enable 2 core options to switch to the less accurate special chip HLE).**

### How to get and install the bsnes-mercury Balanced core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'SNES / Super Famicom (bsnes-mercury Balanced)'.

<center> ![](images\Cores\higan\bsnes_mercury_balanced.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\snes.png) </center>

- If you are asked which core to select, choose 'SNES / Super Famicom (bsnes-mercury Balanced)'.

The content should now start running!

### Authors

- byuu
- Alcaro

## See also

### SNES

- [SNES / Super Famicom (Beetle bsnes)](https://docs.libretro.com/library/beetle_snes/)
- [SNES / Super Famicom (bsnes Accuracy)](https://docs.libretro.com/library/bsnes_accuracy/)
- [SNES / Super Famicom (bsnes Balanced)](https://docs.libretro.com/library/bsnes_balanced/)
- [SNES / Super Famicom (bsnes C++98 (v085))](https://docs.libretro.com/library/bsnes_cplusplus98/)
- [SNES / Super Famicom (bsnes Performance)](https://docs.libretro.com/library/bsnes_performance/)
- [SNES / Super Famicom (bsnes-mercury Accuracy)](https://docs.libretro.com/library/bsnes_mercury_accuracy/)
- [SNES / Super Famicom (bsnes-mercury Performance)](https://docs.libretro.com/library/bsnes_mercury_performance/)
- [SNES / Super Famicom (higan Accuracy)](https://docs.libretro.com/library/higan_accuracy/)
- [SNES / Super Famicom (nSide Balanced)](https://docs.libretro.com/library/nside_balanced/)
- [SNES / Super Famicom (Snes9x 2002)](https://docs.libretro.com/library/snes9x_2002/)
- [SNES / Super Famicom (Snes9x 2005 Plus)](https://docs.libretro.com/library/snes9x_2005_plus/)
- [SNES / Super Famicom (Snes9x 2005)](https://docs.libretro.com/library/snes9x_2005/)
- [SNES / Super Famicom (Snes9x 2010)](https://docs.libretro.com/library/snes9x_2010/)
- [SNES / Super Famicom (Snes9x)](https://docs.libretro.com/library/snes9x/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The bsnes-mercury Balanced core is licensed under

- [GPLv3](https://github.com/libretro/bsnes-mercury/blob/master/LICENSE)

## Extensions

Content that can be loaded by the bsnes-mercury Balanced core have the following file extensions:

- .sfc
- .smc
- .bml

## Databases

RetroArch database(s) that are associated with the bsnes-mercury Balanced core:

- [Nintendo - Super Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System.rdb)
- [Nintendo - Super Nintendo Entertainment System Hacks](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System%20Hacks.rdb)
- [Nintendo - Sufami Turbo](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Sufami%20Turbo.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

!!! attention
	The bsnes-mercury Balanced core uses split ROMS for [special chip games](https://en.wikipedia.org/wiki/List_of_Super_NES_enhancement_chips#List_of_Super_NES_games_that_use_enhancement_chips).

Notable DSP1/DSP1B Games: 

- Super Mario Kart
- Pilotwings

Notable DSP2 Games:

- Dungeon Master

Notable DSP3 Games:

- SD Gundam GX

Notable DSP4 Games: 

- Top Gear 3000

Notable Cx4 Games:

- Mega Man X2
- Mega Man X3

!!! attention
	**The co-processor firmware files for special chip games are only optional when the Allow settings to reduce accuracy core option is enabled and the Special chip accuracy core option is set to HLE. Otherwise, they are required.**

!!! attention
	**The ST-0011 and ST-0018 co-processors cannot be HLE'd.**

|   Filename        |    Description                         |              md5sum              |
|:-----------------:|:--------------------------------------:|:--------------------------------:|
| dsp1.data.rom     | DSP1 co-processor firmware             | 3d81b45fa0c2aa8b852dfb1ece7c0971 |
| dsp1.program.rom  | DSP1 co-processor firmware             | ae209fbe789fbf11a48aea5ab1197321 |
| dsp1b.data.rom    | DSP1B co-processor firmware            | 1e3f568634a7d8284020dddc0ae905bc |
| dsp1b.program.rom | DSP1B co-processor firmware            | d10f446888e097cbf500f3f663cf4f6d |
| dsp2.data.rom     | DSP2 co-processor firmware             | e9417e29223b139c3c4b635a2a3b8744 |
| dsp2.program.rom  | DSP2 co-processor firmware             | aa6e5922a3ed5ded54f24247c11143c5 |
| dsp3.data.rom     | DSP3 co-processor firmware             | 0a81210c0a940b997dd9843281008ee6 |
| dsp3.program.rom  | DSP3 co-processor firmware             | d99ca4562818d49cee1f242705bba6f8 |
| dsp4.data.rom     | DSP4 co-processor firmware             | ee4990879eb68e3cbca239c5bc20303d |
| dsp4.program.rom  | DSP4 co-processor firmware             | a151023b948b90ffc23a5b594bb6fef2 |
| cx4.data.rom      | CX4 co-processor firmware              | 037ac4296b6b6a5c47c440188d3c72e3 |
| st010.data.rom    | ST010 co-processor firmware            | 254d70762b6f59f99c27c395aba7d07d |
| st010.program.rom | ST010 co-processor firmware            | 1d70019179a59a566a0bb5d3f2845544 |
| st011.data.rom    | ST011 co-processor firmware            | 10bd3f4aa949737ab9836512c35bcc29 |
| st011.program.rom | ST011 co-processor firmware            | 95222ebf1c0c2990bcf25db43743f032 |
| st018.data.rom    | ST018 co-processor firmware            | 49c898b60d0f15e90d0ba780dd12f366 |
| st018.program.rom | ST018 co-processor firmware            | dda40ccd57390c96e49d30a041f9a9e7 |
| sgb.boot.rom      | SGB Boot BIOS                          | d574d4f9c12f305074798f54c091a8b4 |

## Features

RetroArch-level settings or features that the bsnes-mercury Balanced core respects.

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
| Subsystem         | ✔         |
| Softpatching      | ✔         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The bsnes-mercury Balanced core's directory name is 'bsnes-mercury'

The bsnes-mercury Balanced core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The bsnes-mercury Balanced core's internal FPS is 60 except for PAL games. PAL games are 50 fps.
- The bsnes-mercury Balanced core's internal sample rate is (Rate)
- The bsnes-mercury Balanced core's core provided aspect ratio is dependent on the ['Preferred aspect ratio' core option](https://docs.libretro.com/library/bsnes_mercury_balanced#core-options).

### Super Gameboy Support

!!! warning
	Super Gameboy support in this core is **command-line only**, **Windows only** and has **buggy save state support** and **visual glitches**. **Use the [higan Accuracy core](https://docs.libretro.com/library/higan_accuracy#super-gameboy-support) or the [nSide Balanced core](https://docs.libretro.com/library/nside_balanced#super-gameboy-support) for simplified, functional, and easily accessible Super Gameboy support.**

Super Gameboy is supported via the Subsystem API. In RetroArch the Subsystem API is only available via [CLI](https://docs.libretro.com/guides/cli-intro/).

For SGB support, you need both the sgb.boot.rom (in RetroArch's system directory) and a SNES Super Game Boy ROM. 

To launch SGB games, launch RetroArch like this:

retroarch -L {path to bsnes core} {path to SNES Super Game Boy ROM} --subsystem sgb {path to GB rom}

!!! warning
	Super Game Boy ROM and GB roms must be unzipped.

### MSU-1 Support

Awaiting description.

## Core options

The bsnes-mercury Balanced core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Allow settings to reduce accuracy** (**Off**/On)

<center> Respect accuracy-impacting settings. </center>

- **Special chip accuracy** (**LLE**/HLE)

<center> Choose whether to use LLE (real BIOS) or HLE (emulated BIOS) for enhancement chips. HLE is less accurate but also less demanding for the special chips. The Allow settings to reduce accuracy core option must be enabled in order for this to function properly. The ST-0011 and ST-0018 co-processors cannot be HLE'd. </center>

- **SuperFX speed** (**100%**/150%/200%/300%/400%/500%/1000%)

<center> Overclock the [SuperFX chip](https://en.wikipedia.org/wiki/Super_FX). 100% is stock clockspeed. The Allow settings to reduce accuracy core option must be enabled in order for this to function properly. </center>

- **System region** (**auto**/ntsc/pal)

<center> Choose which region the system is from. </center>

- **Preferred aspect ratio** (**auto**/ntsc/pal)

<center> Choose the preferred aspect ratio. RetroArch's aspect ratio must be set to Core provided in the Video seetings. </center>

- **Crop overscan** (**Off**/On)

<center> Crop out the potentially random glitchy video output that would have been hidden by the bezel around the edge of a standard-definition television screen. </center>

- **Gamma ramp (requires restart)** (**Off**/On)

<center> Simulates the way a console’s display device differs from modern computer monitor’s colour reproduction. In particular, it simulates the slightly-different gamma correction used by the Super Famicom. </center>

??? note "Gamma ramp - Disabled"
    ![](images/Cores/higan/gamma_off.png)
	
??? note "Gamma ramp - Enabled"
    ![](images/Cores/higan/gamma_on.png)

## Controllers

### Device types

The bsnes-mercury Balanced core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input.
- **[SNES Joypad](http://nintendo.wikia.com/wiki/Super_Nintendo_Entertainment_System_controller)** - Joypad
- [SNES Mouse](https://en.wikipedia.org/wiki/Super_NES_Mouse) - Mouse

#### User 2 device types

- None - Doesn't disable input.
- **[SNES Joypad](http://nintendo.wikia.com/wiki/Super_Nintendo_Entertainment_System_controller)** - Joypad
- [SNES Mouse](https://en.wikipedia.org/wiki/Super_NES_Mouse) - Mouse
- [Multitap](http://nintendo.wikia.com/wiki/Super_Multitap) - Joypad - Allows for up to five players to play together in certain games.
- [SuperScope](https://en.wikipedia.org/wiki/Super_Scope) - Lightgun
- [Justifier](https://en.wikipedia.org/wiki/Konami_Justifier) - Lightgun
- [Justifiers](https://en.wikipedia.org/wiki/Konami_Justifier) - Lightgun - Two Justifiers are plugged in, for two-player Justifier games.

### Multitap support

Activating multitap support in compatible games can be configured by switching to the [Multitap device type](https://docs.libretro.com/library/bsnes_mercury_balanced#controllers) for User 2.

### Controller tables

#### Joypad and analog device type table

| User 1 - 5 Remap descriptors  | RetroPad Inputs                              | SNES Joypad / Multitap |
|-------------------------------|----------------------------------------------|------------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                      |
| Y                             | ![](images/RetroPad/Retro_Y_Round.png)       | Y                      |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select                 |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start                  |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up               |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down             |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left             |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right            |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | A                      |
| X                             | ![](images/RetroPad/Retro_X_Round.png)       | X                      |
| L                             | ![](images/RetroPad/Retro_L1.png)            | L                      |
| R                             | ![](images/RetroPad/Retro_R1.png)            | R                      |

#### Mouse device type table

| User 1 - 2 Remap descriptors  | RetroMouse Inputs                       | SNES Mouse               |
|-------------------------------|------------------------------------------|-------------------------|
|                               | ![](images/RetroMouse/Retro_Mouse.png)   | SNES Mouse Cursor       |
|                               | ![](images/RetroMouse/Retro_Left.png)    | SNES Mouse Left Button  |
|                               | ![](images/RetroMouse/Retro_Right.png)   | SNES Mouse Right Button |

#### Lightgun device type table

| User 2 Remap descriptors      | RetroLightgun Inputs | SuperScope           | Justifier(s)        |
|-------------------------------|----------------------|----------------------|---------------------|
|                               | Gun                  | SuperScope Crosshair | Justifier Crosshair |
|                               | Gun Trigger          | SuperScope Trigger   | Justifier Trigger   |
|                               | Gun Cursor           | SuperScope Cursor    |                     |
|                               | Gun Turbo            | SuperScope Turbo     | Justifier Offscreen |
|                               | Gun Pause            | SuperScope Pause     | Justifier Start     |

## Compatibility

The bsnes-mercury Balanced core fully emulates all SNES games that have ever been officially released. 

## External Links

- [Libretro bsnes-mercury Balanced Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/bsnes_mercury_accuracy_libretro.info)
- [Libretro bsnes-mercury Balanced Github Repository](https://github.com/libretro/bsnes-mercury)
- [Report Libretro bsnes-mercury Balanced Core Issues Here](https://github.com/libretro/bsnes-mercury/issues)
- [Official higan Website](https://byuu.org/)
- [Official higan Upstream Downloads](https://byuu.org/emulation/higan/)