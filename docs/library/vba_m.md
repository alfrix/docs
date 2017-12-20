# Game Boy Advance (VBA-M)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/vba_m.md). Changes are proposed using "Pull Requests."

There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)

## Background

VBA-M is a Game Boy Advance emulator with the goal to improve upon VisualBoyAdvance by integrating the best features from the various builds floating around.

### Why use this core?

Awaiting description.

### How to get and install the VBA-M core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Game Boy Advance (VBA-M)'.

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'Game Boy Advance (VBA-M)'.

The content should now start running!

### Authors

- Forgotten
- VBA-M Team

## See also

- [Game Boy Advance (Beetle GBA)](https://docs.libretro.com/library/beetle_gba/)
- [Game Boy Advance (gpSP)](https://docs.libretro.com/library/gpsp/)
- [Game Boy Advance (Meteor)](https://docs.libretro.com/library/meteor/)
- [Game Boy Advance (mGBA)](https://docs.libretro.com/library/mgba/)
- [Game Boy Advance (VBA Next)](https://docs.libretro.com/library/vba_next/)
- [Game Boy Advance (VBA-M)](https://docs.libretro.com/library/vbam/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

- [GPLv2](https://github.com/libretro/vbam-libretro/blob/master/doc/gpl.txt) 

## Extensions

Content that can be loaded by the VBA-M core have the following file extensions:

- .gba

## Databases

RetroArch database(s) that are associated with the VBA-M core:

- [Nintendo - Game Boy Advance](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Advance.rdb)

## Features

RetroArch features that the VBA-M core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔ (not link-cable emulaion) |
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

The VBA-M core's directory name is 'VBA-M'

The VBA-M core loads from and saves to to these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

The VBA-M core's internal FPS is 59.7275005696

The VBA-M core's internal sample rate is 32000 Hz

The VBA-M core's core provided aspect ratio is 3/2

## Core options

The VBA-M core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Show layer 1** (No/**Yes**)

<center> Self-explanatory. </center>

- **Show layer 2** (No/**Yes**)

<center> Self-explanatory. </center>

- **Show layer 3** (No/**Yes**)

<center> Self-explanatory. </center>

- **Show layer 4** (No/**Yes**)

<center> Self-explanatory. </center>

- **Show sprite layer** (No/**Yes**)

<center> Self-explanatory. </center>

- **Show window layer 1** (No/**Yes**)

<center> Self-explanatory. </center>

- **Show window layer 2** (No/**Yes**)

<center> Self-explanatory. </center>

- **Show sprite window layer** (No/**Yes**)

<center> Self-explanatory. </center>

## Controllers

### Device types

The VBA-M core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Input disabled.
- **RetroPad** - Joypad
- GBA Joypad - Joypad
- Alt Joypad YB - Joypad
- Alt Joypad AB - Joypad

### Controller tables

#### Joypad and analog device type table

| User 1 input descriptors      | RetroPad Inputs                              | RetroPad           | GBA Joypad  | Alt Joypad YB | Alt Joypad AB |
|-------------------------------|----------------------------------------------|--------------------|-------------|---------------|---------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                  | B           | A             |  A            |
| N/A                           | ![](images/RetroPad/Retro_Y_Round.png)       |                    |             | B             |               |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select             | Select      | Select        | Select        |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start              | Start       | Start         | Start         |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up           | D-Pad Up    | D-Pad Up      | D-Pad Up      |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down         | D-Pad Down  | D-Pad Down    | D-Pad Down    |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left         | D-Pad Left  | D-Pad Left    | D-Pad Left    |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right        | D-Pad Right | D-Pad Right   | D-Pad Right   |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | A                  | A           |               | B             |
| L                             | ![](images/RetroPad/Retro_L1.png)            | L                  | L           | L             | L             |
| R                             | ![](images/RetroPad/Retro_R1.png)            | R                  | R           | R             | R             |

## Compatibility

| Game                                  | Issue                          |
|---------------------------------------|--------------------------------|
|**Boktai Trilogy**                     | The solar sensor is not emulated|
|**Digimon Racing (Europe)**            |Freezes during the intro. This can be avoided by enabling linking in the standalone VBA-M release  |
|**Koro Koro Puzzle Happy Panechu!**    |	The tilt sensor is not emulated|
|**Phantasy Star Collection**           | Digital Eclipse logo sound effect is missing. Phantasy Star 1 flickers |
|**WarioWare: Twisted!**                |  	The tilt sensor is not emulated   |
|**Yoshi’s Universal Gravitation**      |   The tilt sensor is not emulated   |

## External Links

- [Libretro VBA-M Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/vbam_libretro.info)
- [Libretro VBA-M Github Repository](https://github.com/libretro/vbam-libretro)
- [Report Libretro VBA-M Core Issues Here](https://github.com/libretro/vbam-libretro/issues)
- [Official VBA-M Website](http://vba-m.com/)
- [Official VBA-M Github Repository](https://github.com/visualboyadvance-m/visualboyadvance-m)