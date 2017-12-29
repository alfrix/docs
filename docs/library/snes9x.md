# SNES / Super Famicom (Snes9x)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/snes9x.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Port of upstream mainline **up-to-date** Snes9x, a portable Super Nintendo Entertainment System emulator to libretro.

### Why use this core?

- Highly accurate SNES emulation.
- Simplified and easily accessible MSU-1 expansion chip support.
- Recommended for netplay
- Less CPU intensive than the higan/bsnes based cores.
- **Most up-to-date libretro Snes9x core available.**

### How to get and install the Snes9x core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'SNES / Super Famicom (Snes9x)'.

<center> ![](images\Cores\snes9x\snes9x.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\snes.png) </center>

- If you are asked which core to select, choose 'SNES / Super Famicom (Snes9x)'.

The content should now start running!

### Authors

- Snes9x Team

## See also

### SNES

- [SNES / Super Famicom (Beetle bsnes)](https://docs.libretro.com/library/beetle_snes/)
- [SNES / Super Famicom (bsnes Accuracy)](https://docs.libretro.com/library/bsnes_accuracy/)
- [SNES / Super Famicom (bsnes Balanced)](https://docs.libretro.com/library/bsnes_balanced/)
- [SNES / Super Famicom (bsnes C++98 (v085))](https://docs.libretro.com/library/bsnes_cplusplus98/)
- [SNES / Super Famicom (bsnes Performance)](https://docs.libretro.com/library/bsnes_performance/)
- [SNES / Super Famicom (bsnes-mercury Accuracy)](https://docs.libretro.com/library/bsnes_mercury_accuracy/)
- [SNES / Super Famicom (bsnes-mercury Balanced)](https://docs.libretro.com/library/bsnes_mercury_balanced/)
- [SNES / Super Famicom (bsnes-mercury Performance)](https://docs.libretro.com/library/bsnes_mercury_performance/)
- [SNES / Super Famicom (higan Accuracy)](https://docs.libretro.com/library/higan_accuracy/)
- [SNES / Super Famicom (nSide Balanced)](https://docs.libretro.com/library/nside/)
- [SNES / Super Famicom (Snes9x 2002)](https://docs.libretro.com/library/snes9x_2002/)
- [SNES / Super Famicom (Snes9x 2005 Plus)](https://docs.libretro.com/library/snes9x_2005_plus/)
- [SNES / Super Famicom (Snes9x 2005)](https://docs.libretro.com/library/snes9x_2005/)
- [SNES / Super Famicom (Snes9x 2010)](https://docs.libretro.com/library/snes9x_2010/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Snes9x core is licensed under

- [Non-commercial](https://github.com/libretro/snes9x/blob/master/docs/snes9x-license.txt)

## Extensions

Content that can be loaded by the Snes9x core have the following file extensions:

- .smc
- .sfc
- .swc
- .fig

## Databases

RetroArch database(s) that are associated with the Snes9x core:

- [Nintendo - Super Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System.rdb)
- [Nintendo - Super Nintendo Entertainment System Hacks](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System%20Hacks.rdb)
- [Nintendo - Sufami Turbo](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Sufami%20Turbo.rdb)

## Features

RetroArch-level settings or features that the Snes9x core respects.

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
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| Softpatching      | ✔         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The Snes9x core's directory name is 'Snes9x'

The Snes9x core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The Snes9x core's internal FPS is 60 except for PAL games. PAL games are 50 fps.
- The Snes9x core's internal sample rate is 32040 Hz
- The Snes9x core's core provided aspect ratio is dependent on the ['Preferred aspect ratio' core option](https://docs.libretro.com/library/snes9x#core-options).

### MSU-1 support

MSU-1 support in the Snes9x core follows the SD2SNES naming format, i.e.
```
gamename\
gamename.sfc
gamename.msu
gamename-#.pcm
```

Loading a manifest.bml file or having a xml file isn't necessary. **Just load gamename.sfc.**

Here's an example of a working MSU-1 setup done with Secret of Mana MSU-1. Please note that som_msu1.sfc is being [softpatched](https://docs.libretro.com/guides/softpatching/) in this example.

![](images/Cores/snes9x/msu.png)

## Core options

The Snes9x core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **SuperFX Frequency** (**10MHz**/20MHz/40MHz/60MHz/80MHz/100MHz)

<center> Overclock the [SuperFX chip](https://en.wikipedia.org/wiki/Super_FX). 10Mhz is stock clockspeed. </center>

- **Show layer 1** (Off/**On**)

<center> Self-explanatory. </center>

- **Show layer 2** (Off/**On**)

<center> Self-explanatory. </center>

- **Show layer 3** (Off/**On**)

<center>Self-explanatory. </center>

- **Show layer 4** (Off/**On**)

<center> Self-explanatory. </center>

- **Show sprite layer** (Off/**On**)

<center> Self-explanatory. </center>

- **Enable graphic clip windows** (Off/**On**)

<center> Self-explanatory. </center>

- **Enable transparency effects** (Off/**On**)

<center> Self-explanatory. </center>

- **Enable sound channel 1** (Off/**On**)

<center> Self-explanatory. </center>

- **Enable sound channel 2** (Off/**On**)

<center> Self-explanatory. </center>

- **Enable sound channel 3** (Off/**On**)

<center> Self-explanatory. </center>

- **Enable sound channel 4** (Off/**On**)

<center> Self-explanatory. </center>

- **Enable sound channel 5** (Off/**On**)

<center> Self-explanatory. </center>

- **Enable sound channel 6** (Off/**On**)

<center> Self-explanatory. </center>

- **Enable sound channel 7** (Off/**On**)

<center> Self-explanatory. </center>

- **Enable sound channel 8** (Off/**On**)

<center> Self-explanatory. </center>

- **Crop overscan** (**auto**/On/Off)

<center> Crop out the potentially random glitchy video output that would have been hidden by the bezel around the edge of a standard-definition television screen. </center>

??? note "Crop overscan - On"
	![](images\Cores\snes9x\crop_on.png)
	
??? note "Crop overscan - Off"
	![](images\Cores\snes9x\crop_off.png)	

- **Preferred aspect ratio** (**auto**/ntsc/pal/4:3)

<center> Choose the preferred aspect ratio. RetroArch's aspect ratio must be set to Core provided in the Video seetings. </center>

??? note "Preferred aspect ratio - ntsc"
	![](images\Cores\snes9x\ntsc.png)
	
??? note "Preferred aspect ratio - pal"
	![](images\Cores\snes9x\pal.png)

??? note "Preferred aspect ratio - 4:3"
	![](images\Cores\snes9x\4by3.png)	

## Controllers

### Device types

The Snes9x core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input.
- **[SNES Joypad](http://nintendo.wikia.com/wiki/Super_Nintendo_Entertainment_System_controller)** - Joypad
- [SNES Mouse](https://en.wikipedia.org/wiki/Super_NES_Mouse) - Mouse
- [Multitap](http://nintendo.wikia.com/wiki/Super_Multitap) - Joypad - Allows for up to five players to play together in certain games.

#### User 2 device types

- None - Doesn't disable input.
- **[SNES Joypad](http://nintendo.wikia.com/wiki/Super_Nintendo_Entertainment_System_controller)** - Joypad
- [SNES Mouse](https://en.wikipedia.org/wiki/Super_NES_Mouse) - Mouse
- [Multitap](http://nintendo.wikia.com/wiki/Super_Multitap) - Joypad - Allows for up to five players to play together in certain games.
- [SuperScope](https://en.wikipedia.org/wiki/Super_Scope) - Lightgun
- [Justifier](https://en.wikipedia.org/wiki/Konami_Justifier) - Lightgun

### Multitap support

Activating multitap support in compatible games can be configured by switching to the [Multitap device types](https://docs.libretro.com/library/snes9x#controllers) for the corresponding users.

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

| User 1 - 2 Input descriptors  | RetroMouse Inputs                        | SNES Mouse         |
|-------------------------------|------------------------------------------|--------------------|
|                               | ![](images/RetroMouse/Retro_Mouse.png)   | SNES Mouse Cursor  |
|                               | ![](images/RetroMouse/Retro_Left.png)    | SNES Left Button   |
|                               | ![](images/RetroMouse/Retro_Right.png)   | SNES Right Button  |

#### Lightgun device type table

| User 1 - 2 Input descriptors  | RetroLightgun Inputs | SuperScope           | Justifier           |
|-------------------------------|----------------------|----------------------|---------------------|
|                               | Gun                  | SuperScope Crosshair | Justifier Crosshair |
|                               | Gun Trigger          | SuperScope Trigger   | Justifier Trigger   |
|                               | Gun Cursor           | SuperScope Cursor    |                     |
|                               | Gun Turbo            | SuperScope Turbo     | Justifier Offscreen |
|                               | Gun Pause            | SuperScope Pause     | Justifier Start     |

!!! attention
	All of the Super Scope games made by Nintendo have a soft-reset to the game's main title. This is accomplished by pausing the game, then, while holding Cursor, the Fire button must be pressed twice.

## Compatibility

| Game                                             | Issue                                                                                |
|--------------------------------------------------|--------------------------------------------------------------------------------------|
| A.S.P. Air Strike Patrol                         | The shadow below the aircraft is missing. Glitched graphics on the briefing screens. |
| BS-Zelda MottZilla Patch                         | Only shows a black screen.                                                           |
| Doom                                             | Colored dots appear during gameplay.                                                 |
| Funaki Masakatsu Hybrid Wrestler – Tougi Denshou | Corrupted graphics on the Pancrase logo screen.                                      |
| Hayazashi Nidan Morita Shougi 2                  | Matches won’t start.                                                                 |
| Mecarobot Golf                                   | The ground "wobbles" during gameplay.                                                |
| Secret of Evermore (PAL versions)                | Randomly freezes when the background music changes.                                  |
| Speedy Gonzales: Los Gatos Bandidos              | Freezes when pressing a switch in the last level.                                    |

!!! attention
	The Snes9x core can launch some Satellaview games with sometimes low compatibility.

## External Links

- [Libretro Snes9x Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/snes9x_libretro.info)
- [Libretro Snes9x Github Repository](https://github.com/libretro/snes9x)
- [Report Libretro Snes9x Core Issues Here](https://github.com/libretro/snes9x/issues)
- [Official Snes9x Website (no longer updated)](http://www.snes9x.com/)
- [Official Snes9x Github Repository](https://github.com/snes9xgit/snes9x)
- [Official Upstream Snes9x Downloads](http://www.s9x-w32.de/dl/)
- [Alternate Official Upstream Snes9x Downloads](https://sites.google.com/site/bearoso/)