# SNES / Super Famicom (Snes9x 2005 Plus)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/snes9x_2005_plus.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Port of SNES9x 1.43 for libretro

This core is part of a group of Snes9x cores that are snapshots from the year their code is based on. (Snes9x 2002, Snes9x 2005, Snes9x 2005 Plus, Snes9x 2010)

This core has been compiled with Blargg's APU

### Why use this core?

- Provides more favorable performance thresholds at the cost of accuracy. **DO NOT use this core unless you have underpowered hardware and the mainline Snes9x core and the bsnes/higan/bsnes-mercury cores aren't fast enough**

### How to get and install the Snes9x 2005 Plus core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'SNES / Super Famicom (Snes9x 2005 Plus)'.

<center> ![](images\Cores\snes9x\snes9x_2005_plus.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\snes.png) </center>

- If you are asked which core to select, choose '(Title)'.

The content should now start running!

### Authors

- Snes9x Team
- dking
- BassAceGold
- ShadauxCat
- Nebuleon

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
- [SNES / Super Famicom (Snes9x 2005)](https://docs.libretro.com/library/snes9x_2005/)
- [SNES / Super Famicom (Snes9x 2010)](https://docs.libretro.com/library/snes9x_2010/)
- [SNES / Super Famicom (Snes9x)](https://docs.libretro.com/library/snes9x/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Snes9x 2005 Plus core is licensed under

- [Non-commercial](https://github.com/libretro/snes9x/blob/master/docs/snes9x-license.txt)

## Extensions

Content that can be loaded by the Snes9x 2005 Plus core have the following file extensions:

- .smc
- .fig
- .sfc
- .gd3
- .gd7
- .dx2
- .bsx
- .swc

## Databases

RetroArch database(s) that are associated with the Snes9x 2005 Plus core:

- [Nintendo - Super Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System.rdb)
- [Nintendo - Super Nintendo Entertainment System Hacks](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System%20Hacks.rdb)
- [Nintendo - Sufami Turbo](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Sufami%20Turbo.rdb)

## Features

RetroArch-level settings or features that the Snes9x 2005 Plus core respects.

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
| Softpatching      | ✔         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The Snes9x 2005 Plus core's directory name is 'Snes9x 2005 Plus'

The Snes9x 2005 Plus core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The Snes9x 2005 Plus core's internal FPS is (FPS)
- The Snes9x 2005 Plus core's internal sample rate is (Rate)
- The Snes9x 2005 Plus core's core provided aspect ratio is 4/3

## Core options

The Snes9x 2005 Plus core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Video Mode** (**auto**/NTSC/PAL)

<center> Awaiting description. </center>

## Controllers

### Device types

The Snes9x 2005 Plus core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 5 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There's no reason to switch to this.

### Controller tables

#### Joypad and analog device type table

| User 1 - 5 Input descriptors  | RetroPad Inputs                              |
|-------------------------------|----------------------------------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       |
| Y                             | ![](images/RetroPad/Retro_Y_Round.png)       |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | 
| Start                         | ![](images/RetroPad/Retro_Start.png)         |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | 
| A                             | ![](images/RetroPad/Retro_A_Round.png)       |
| X                             | ![](images/RetroPad/Retro_X_Round.png)       | 
| L                             | ![](images/RetroPad/Retro_L1.png)            |
| R                             | ![](images/RetroPad/Retro_R1.png)            |

## Compatibility

| Game                                             | Issue                                                                                |
|--------------------------------------------------|--------------------------------------------------------------------------------------|
| A.S.P. Air Strike Patrol                         | The shadow below the aircraft is missing. Glitched graphics on the briefing screens. |
| Bass Masters Classic - Pro Edition               | Only shows a black screen.                                                           |
| Funaki Masakatsu Hybrid Wrestler – Tougi Denshou | Corrupted graphics on the Pancrase logo screen.                                      |
| Hayazashi Nidan Morita Shougi 2                  | Matches won’t start.                                                                 |
| Madden NFL 96                                    | Only shows a black screen.                                                           |
| Masters New – Harukanaru Augusta 3               | Black screen after selecting game.                                                   |
| Mecarobot Golf                                   | The ground "wobbles" during gameplay.                                               |
| Mechwarrior 3050                                 | Black screen after the Activision logo.                                              |

## External Links

- [Libretro Snes9x 2005 Plus Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/snes9x2005_plus_libretro.info)
- [Libretro Snes9x 2005 Plus Github Repository](https://github.com/libretro/snes9x2005)
- [Report Libretro Snes9x 2005 Plus Core Issues Here](https://github.com/libretro/snes9x2005/issues)
- [Official Snes9x 2005 Plus Github Repository](https://github.com/ShadauxCat/CATSFC)