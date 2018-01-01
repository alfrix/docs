# Neo Geo Pocket/Color (Beetle NeoPop)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_neopop.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Beetle/Mednafen NGP is a SNK Neo Geo Pocket (Color) video game system emulator based on NeoPop

### Why use this core?

Awaiting description.

### How to get and install the Beetle NeoPop core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Neo Geo Pocket/Color (Beetle NeoPop)'.

<center> ![](images\Cores\beetle_neopop\beetle_neopop.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\ngp.png) </center>

- If you are asked which core to select, choose 'Neo Geo Pocket/Color (Beetle NeoPop)'.

The content should now start running!

### Authors

- neopop_uk
- [Mednafen Team](https://mednafen.github.io/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Beetle NeoPop core is licensed under

- [GPLv2](https://github.com/libretro/beetle-ngp-libretro/blob/master/COPYING)

## Extensions

Content that can be loaded by the Beetle NeoPop core have the following file extensions:

- .ngp
- .ngc

## Databases

RetroArch database(s) that are associated with the Beetle NeoPop core:

- [SNK - Neo Geo Pocket](https://github.com/libretro/libretro-database/blob/master/rdb/SNK%20-%20Neo%20Geo%20Pocket.rdb)
- [SNK - Neo Geo Pocket Color](https://github.com/libretro/libretro-database/blob/master/rdb/SNK%20-%20Neo%20Geo%20Pocket%20Color.rdb)

## Features

RetroArch-level settings or features that the Beetle NeoPop core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔ (not link-cable emulation) |
| Core Options      | ✔         |
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
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | ✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✔         |

### Directories

The Beetle NeoPop core's directory name is 'Mednafen NeoPop'

The Beetle NeoPop core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.flash (Cartrtidge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The Beetle NeoPop core's internal FPS is 60
- The Beetle NeoPop core's internal sample rate is 44100 Hz
- The Beetle NeoPop core's core provided aspect ratio is 20/19

## Core options

The Beetle NeoPop core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Language (restart)** (**english**/japanese)

 Choose system language of the BIOS.

## Controllers

### Device types

The Beetle NeoPop core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There's no reason to switch to this.

### Controller tables

#### Joypad and analog device type table

| User 1 Remap descriptors      | RetroPad Inputs                              |
|-------------------------------|----------------------------------------------|
| A                             | ![](images/RetroPad/Retro_B_Round.png)       |
| Option                        | ![](images/RetroPad/Retro_Start.png)         |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    |
| B                             | ![](images/RetroPad/Retro_A_Round.png)       |

## Compatibility

Awaiting description.

## External Links

- [Libretro Beetle NeoPop Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_ngp_libretro.info)
- [Libretro Beetle NeoPop Github Repository](https://github.com/libretro/beetle-ngp-libretro)
- [Report Libretro Beetle NeoPop Core Issues Here](https://github.com/libretro/beetle-ngp-libretro/issues)
- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)