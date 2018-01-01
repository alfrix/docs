# SNES / Super Famicom (bsnes C++98 (v085))

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/bsnes_cplusplus98.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

bsnes c++98 is a special fork from around v085 that's been backported to work with older compilers. Many platforms Libretro supports such as various consoles (PlayStation 3) are stuck with super-old compilers that don't support the latest c++ features that are in the newer bsnes v094 ports.

### Why use this core?

There's no reason to use this core now expect for edge cases on less compatible platforms.

### How to get and install the bsnes C++98 (v085) core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'SNES / Super Famicom (bsnes C++98 (v085))'.

<center> ![](images\Cores\higan\bsnes_cplusplus98.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\snes.png) </center>

- If you are asked which core to select, choose 'SNES / Super Famicom (bsnes C++98 (v085))'.

The content should now start running!

### Authors

- byuu
- Themaister
- Ver GreenEyes

## See also

### SNES

- [SNES / Super Famicom (Beetle bsnes)](https://docs.libretro.com/library/beetle_bsnes/)
- [SNES / Super Famicom (bsnes Accuracy)](https://docs.libretro.com/library/bsnes_accuracy/)
- [SNES / Super Famicom (bsnes Balanced)](https://docs.libretro.com/library/bsnes_balanced/)
- [SNES / Super Famicom (bsnes Performance)](https://docs.libretro.com/library/bsnes_performance/)
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

The bsnes C++98 (v085) core is licensed under

- [GPLv3](https://github.com/libretro/bsnes-libretro/blob/libretro/COPYING)

## Extensions

Content that can be loaded by the bsnes C++98 (v085) core have the following file extensions:

- .sfc
- .smc

## Databases

RetroArch database(s) that are associated with the bsnes C++98 (v085) core:

- [Nintendo - Super Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System.rdb)
- [Nintendo - Super Nintendo Entertainment System Hacks](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System%20Hacks.rdb)
- [Nintendo - Sufami Turbo](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Sufami%20Turbo.rdb)

## Features

RetroArch-level settings or features that the bsnes C++98 (v085) core respects.

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
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | -         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| Softpatching      | ✔         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✔         |

### Directories

The bsnes C++98 (v085) core's directory name is 'bSNES'

The bsnes C++98 (v085) core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The bsnes C++98 (v085) core's internal FPS is 60 except for PAL games. PAL games are 50 fps.
- The bsnes C++98 (v085) core's internal sample rate is (Rate)
- The bsnes C++98 (v085) core's core provided aspect ratio is (Ratio)

## Controllers

### Device types

The bsnes C++98 (v085) core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

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

Activating multitap support in compatible games can be configured by switching to the [Multitap device type](https://docs.libretro.com/library/bsnes_cplusplus98#controllers) for User 2.

### Controller tables

#### Joypad and analog device type table

| User 1 - 5 Input descriptors  | RetroPad Inputs                              | SNES Joypad / Multitap |
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

| User 1 - 2 Input descriptors  | RetroMouse Inputs                       | SNES Mouse               |
|-------------------------------|------------------------------------------|-------------------------|
|                               | ![](images/RetroMouse/Retro_Mouse.png)   | SNES Mouse Cursor       |
|                               | ![](images/RetroMouse/Retro_Left.png)    | SNES Mouse Left Button  |
|                               | ![](images/RetroMouse/Retro_Right.png)   | SNES Mouse Right Button |

#### Lightgun device type table

| User 2 Input descriptors      | RetroLightgun Inputs | SuperScope           | Justifier(s)        |
|-------------------------------|----------------------|----------------------|---------------------|
|                               | Gun                  | SuperScope Crosshair | Justifier Crosshair |
|                               | Gun Trigger          | SuperScope Trigger   | Justifier Trigger   |
|                               | Gun Cursor           | SuperScope Cursor    |                     |
|                               | Gun Turbo            | SuperScope Turbo     | Justifier Offscreen |
|                               | Gun Pause            | SuperScope Pause     | Justifier Start     |

!!! attention
	All of the Super Scope games made by Nintendo have a soft-reset to the game's main title. This is accomplished by pausing the game, then, while holding Cursor, the Fire button must be pressed twice.

## Compatibility

Awaiting description.

## External Links

- [Libretro bsnes C++98 (v085) Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/bsnes_cplusplus98_libretro.info)
- [Libretro bsnes C++98 (v085) Github Repository](https://github.com/libretro/bsnes-libretro-cplusplus98)
- [Report Libretro bsnes C++98 (v085) Core Issues Here](https://github.com/libretro/bsnes-libretro-cplusplus98/issues)
- [Official higan Website](https://byuu.org/)
- [Official higan Upstream Downloads](https://byuu.org/emulation/higan/)