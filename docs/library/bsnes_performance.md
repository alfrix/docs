# SNES / Super Famicom (bsnes Performance)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/bsnes_performance.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

bsnes is a Super Nintendo emulator that began development on 2004-10-14. It focuses on accuracy and clean code above all else. It never uses speed or compatibilty hacks. As a result, the minimum system requirements are greater than with other emulators. bsnes comes in three different profiles (accuracy, balanced and performance) which contain minor differences in the PPU (graphics) emulation. 

This core has been compiled with the Performance profile.

### Why use this core?

Highly accurate SNES emulation. Whether to use the Accuracy, or Balanced or Performance core depends on how much accuracy you want to give up for game performance. Please check the [compatibility section](https://docs.libretro.com/library/bsnes_performance/#compatibility) for more information.

### How to get and install the bsnes Performance core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'SNES / Super Famicom (bsnes Performance)'.

<center> ![](images\Cores\higan\bsnes_performance.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\snes.png) </center>

- If you are asked which core to select, choose 'SNES / Super Famicom (bsnes Performance)'.

The content should now start running!

### Authors

- byuu

## See also

### SNES

- [SNES / Super Famicom (Beetle bsnes)](https://docs.libretro.com/library/beetle_snes/)
- [SNES / Super Famicom (bsnes Accuracy)](https://docs.libretro.com/library/bsnes_accuracy/)
- [SNES / Super Famicom (bsnes Balanced)](https://docs.libretro.com/library/bsnes_balanced/)
- [SNES / Super Famicom (bsnes C++98 (v085))](https://docs.libretro.com/library/bsnes_cplusplus98/)
- [SNES / Super Famicom (bsnes-mercury Accuracy)](https://docs.libretro.com/library/bsnes_mercury_accuracy/)
- [SNES / Super Famicom (bsnes-mercury Balanced)](https://docs.libretro.com/library/bsnes_mercury_balanced/)
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

The bsnes Performance core is licensed under

- [GPLv3](https://github.com/libretro/bsnes-libretro/blob/libretro/COPYING)

## Extensions

Content that can be loaded by the bsnes Performance core have the following file extensions:

- .sfc
- .smc
- .bml

## Databases

RetroArch database(s) that are associated with the bsnes Performance core

- [Nintendo - Super Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System.rdb)
- [Nintendo - Super Nintendo Entertainment System Hacks](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System%20Hacks.rdb)
- [Nintendo - Sufami Turbo](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Sufami%20Turbo.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

!!! attention
	The bsnes Performance core uses split ROMS for [special chip games](https://en.wikipedia.org/wiki/List_of_Super_NES_enhancement_chips#List_of_Super_NES_games_that_use_enhancement_chips).

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
| sgb.boot.rom      | Super Game Boy 1 or 2 BIOS             |                                  |

## Features

RetroArch-level settings or features that the bsnes Peformance core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| Core Options      | ✕         |
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
| Crop Overscan     | ✔         |

### Directories

The bsnes Performance core's directory name is 'bsnes'

The bsnes Performance core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The bsnes Performance core's internal FPS is 60 except for PAL games. PAL games are 50 fps.
- The bsnes Performance core's internal sample rate is 32040 Hz
- The bsnes Performance core's core provided aspect ratio is 4/3

### Super Gameboy Support

!!! warning
	Super Gameboy support in this core is **command-line only**, **Windows only** and has **buggy save state support** and **visual glitches**. **Use the [higan Accuracy core](https://docs.libretro.com/library/higan_accuracy#super-gameboy-support) or the [nSide Balanced core](https://docs.libretro.com/library/nside_balanced#super-gameboy-support) for simplified, functional, and easily accessible Super Gameboy support.**

Super Gameboy is supported via the Subsystem API. In RetroArch the Subsystem API is only available via [CLI](https://buildbot.libretro.com/docs/guides/cli-intro/).

For SGB support, you need both the sgb.boot.rom (in RetroArch's system directory) and a SNES Super Game Boy ROM. 

To launch SGB games, launch RetroArch like this:

retroarch -L {path to bsnes core} {path to SNES Super Game Boy ROM} --subsystem sgb {path to GB rom}

!!! warning
	Super Game Boy ROM and GB roms must be unzipped.

### MSU-1 Support

Awaiting description.

## Controllers

### Device types

The bsnes Performance core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

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

Activating multitap support in compatible games can be configured by switching to the [Multitap device type](https://docs.libretro.com/library/bsnes_performance#controllers) for User 2.

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

| Game                                             | Issue                                                                          |
|--------------------------------------------------|--------------------------------------------------------------------------------|
| A.S.P. Air Strike Patrol                         | Black lines show up during gameplay. The shadow below the aircraft is missing. |
| Funaki Masakatsu Hybrid Wrestler – Tougi Denshou | Corrupted graphics on the Pancrase logo screen.                                |
| Mecarobot Golf                                   | The ground "wobbles" during gameplay.                                          |
| Mega Man X2                                      | Only displays a black screen.                                                  |
| Mega Man X3                                      | Only displays a black screen.                                                  |
| Mortal Kombat II                                 | Various glitched graphics.                                                     |
| NHL ’94                                          | Corrupted line on the NHL logo screen.                                         |
| Tetris Attack                                    | Lots of flickering on the VS. CPU mode map screen.                             |

## External Links

- [Libretro bsnes Performance Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/bsnes_performance_libretro.info)
- [Libretro bsnes Performance Github Repository](https://github.com/libretro/bsnes-libretro)
- [Report Libretro bsnes Performance Core Issues Here](https://github.com/libretro/bsnes-libretro/issues)
- [Official higan Website](https://byuu.org/)
- [Official higan Upstream Downloads](https://byuu.org/emulation/higan/)