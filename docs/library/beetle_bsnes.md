# SNES / Super Famicom (Beetle bsnes)

## Contribute to this documentation

**DOCUMENTATION IS A WORK IN PROGRESS**

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_bsnes.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Standalone port of Mednafen bSNES to libretro, itself a old fork of bsnes 0.59.

### Why use this core?

This core exists as a side effect of porting/forking mednafen for its other cores in the past. There's no reason to use this core now that there's other more compatible and faster SNES cores.

### How to install the Beetle bsnes core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'SNES / Super Famicom (Beetle bsnes)'.

<center> ![](images\Cores\updater\beetle_bsnes.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start the Beetle bsnes core:

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

- If you are asked which core to select, choose 'SNES / Super Famicom (Beetle bsnes)'.

The content should now start running!

### Authors

- byuu
- [Mednafen Team](https://mednafen.github.io/)

## See also

### SNES

- [SNES / Super Famicom (bsnes Accuracy)](https://docs.libretro.com/library/bsnes_accuracy/)
- [SNES / Super Famicom (bsnes Balanced)](https://docs.libretro.com/library/bsnes_balanced/)
- [SNES / Super Famicom (bsnes C++98 (v085))](https://docs.libretro.com/library/bsnes_cplusplus98/)
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

The Beetle bsnes core is licensed under

- [GPLv2](https://github.com/libretro/beetle-bsnes-libretro/blob/master/COPYING)

## Extensions

Content that can be loaded by the Beetle bsnes core have the following file extensions:

- .smc
- .fig
- .bs
- .st
- .sfc

## Databases

RetroArch database(s) that are associated with the Beetle bsnes core:

- [Nintendo - Super Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System.rdb)
- [Nintendo - Super Nintendo Entertainment System Hacks](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System%20Hacks.rdb)
- [Nintendo - Sufami Turbo](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Sufami%20Turbo.rdb)

## Features

RetroArch-level settings or features that the Beetle bsnes core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| Core Options      | ✕         |
| RetroAchievements | ✕         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✕         |
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | ✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✔         |
| LEDs              | ✕         |

### Directories

The Beetle bsnes core's directory name is 'Mednafen bSNES'

The Beetle bsnes core saves/loads to/from these directories.

**RetroArch's Config directory**

- Mednafen bSNES.cfg (Core Overrides)
- 'content-name'.cfg (Game Overrides)
- 'content-name'.opt (Game-options)

**RetroArch's Input Remapping directory**

- Mednafen bSNES.rmp (Core Remap)
- 'content-name'.rmp (Game Remap)

**RetroArch's Video Shader directory**

- Mednafen bSNES.'shader-preset-extension' (Core Shader Preset)
- 'content-name'.'shader-preset-extension' (Game Shader Preset)

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)
- 'content-name'.rtc (Real time clock save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The Beetle bsnes core's core provided FPS is 60
- The Beetle bsnes core's core provided sample rate is 44100 Hz
- The Beetle bsnes core's core provided aspect ratio is 4/3

## Controllers

The Beetle bsnes core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User # - # device types

- None - Doesn't disable input
- **RetroPad** - Joypad
- RetroPad w/Analog  - Joypad - There's no reason to switch to this.

### Controller tables

#### Joypad

| User # Remap descriptors | RetroPad Inputs                              | RetroPad      |
|--------------------------|----------------------------------------------|---------------|
|                          | ![](images/RetroPad/Retro_B_Round.png)       | B             |
|                          | ![](images/RetroPad/Retro_Y_Round.png)       | Y             |
|                          | ![](images/RetroPad/Retro_Select.png)        | Select        |
|                          | ![](images/RetroPad/Retro_Start.png)         | Start         |
|                          | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up      |
|                          | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down    |
|                          | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left    |
|                          | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right   |
|                          | ![](images/RetroPad/Retro_A_Round.png)       | A             |
|                          | ![](images/RetroPad/Retro_X_Round.png)       | X             |
|                          | ![](images/RetroPad/Retro_L1.png)            | L             |
|                          | ![](images/RetroPad/Retro_R1.png)            | R             |

## Compatibility

Awaiting description.

## External Links

- [Libretro Beetle bsnes Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_snes_libretro.info)
- [Libretro Beetle bsnes Github Repository](https://github.com/libretro/beetle-bsnes-libretro)
- [Report Libretro Beetle bsnes Core Issues Here](https://github.com/libretro/beetle-bsnes-libretro/issues)
- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)