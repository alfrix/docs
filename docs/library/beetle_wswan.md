# WonderSwan/Color (Beetle Cygne)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/). Changes are proposed using "Pull Requests."**

// Add (core-doc-filename).md to the end of the URL.

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Standalone port of Mednafen WonderSwan to libretro, itself a fork of Cygne. 

### Why use this core?

Awaiting description.

### How to get and install the Beetle Cygne core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'WonderSwan/Color (Beetle Cygne)'.

<center> ![](images\Cores\beetle_cygne\cygne.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

- If you are asked which core to select, choose 'WonderSwan/Color (Beetle Cygne)'.

The content should now start running!

### Authors

- Dox
- [Mednafen Team](https://mednafen.github.io/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Beetle Cygne core is licensed under

- [GPLv2](https://github.com/libretro/beetle-wswan-libretro/blob/master/COPYING)

## Extensions

Content that can be loaded by the Beetle Cygne core have the following file extensions:

- .ws
- .wsc

## Databases

RetroArch database(s) that are associated with the Beetle Cygne core:

- [Bandai - WonderSwan](https://github.com/libretro/libretro-database/blob/master/rdb/Bandai%20-%20WonderSwan.rdb)
- [Bandai - WonderSwan Color](https://github.com/libretro/libretro-database/blob/master/rdb/Bandai%20-%20WonderSwan%20Color.rdb)

## Features

RetroArch-level settings or features that the Beetle Cygne core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔ (not link-cable emulation) |
| Core Options      | ✕         |
| RetroAchievements | ✕         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | ✕         |
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

The Beetle Cygne core's directory name is 'Mednafen WonderSwan'

The Beetle Cygne core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.sav (Cartridge backup save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The Beetle Cygne core's internal FPS is 75.47
- The Beetle Cygne core's internal sample rate is 44100 Hz
- The Beetle Cygne core's core provided aspect ratio is 14/9

## Controllers

### Device types

The Beetle Cygne core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog - There is no reason to switch to this.

### Controller tables

#### Joypad and analog device type table

| User 1 Input descriptors      | RetroPad Inputs                              | RetroPad                           |
|-------------------------------|----------------------------------------------|------------------------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                                  |
|                               | ![](images/RetroPad/Retro_Select.png)        | Rotate screen and the active D-Pad |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start                              |
| X Cursor Up                   | ![](images/RetroPad/Retro_Dpad_Up.png)       | X Cursor Up                        |
| X Cursor Down                 | ![](images/RetroPad/Retro_Dpad_Down.png)     | X Cursor Down                      |
| X Cursor Left                 | ![](images/RetroPad/Retro_Dpad_Left.png)     | X Cursor Left                      |
| X Cursor Right                | ![](images/RetroPad/Retro_Dpad_Right.png)    | X Cursor Right                     |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | A                                  |
| Y Cursor Left                 | ![](images/RetroPad/Retro_L1.png)            | Y Cursor Left                      |
| Y Cursor Right                | ![](images/RetroPad/Retro_R1.png)            | Y Cursor Right                     |
| Y Cursor Down                 | ![](images/RetroPad/Retro_L2.png)            | Y Cursor Down                      |
| Y Cursor Up                   | ![](images/RetroPad/Retro_R2.png)            | Y Cursor Up                        |

## Compatibility

| Game      | Issue                                                                        |
|-----------|------------------------------------------------------------------------------|
| Tonpuusou | Title screen announcer voice missing. Softlocks after picking a menu option. |

## External Links

- [Libretro Beetle Cygne Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_wswan_libretro.info)
- [Libretro Beetle Cygne Github Repository](https://github.com/libretro/beetle-wswan-libretro)
- [Report Libretro Beetle Cygne Core Issues Here](https://github.com/libretro/beetle-wswan-libretro/issues)
- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)