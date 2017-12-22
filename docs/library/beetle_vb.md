# Virtual Boy (Beetle VB)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_vb.md). Changes are proposed using "Pull Requests."

There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)

You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).

## Background

Port of Mednafen VB to libretro.

### Why use this core?

Awaiting description.

### How to get and install the Beetle VB core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Virtual Boy (Beetle VB)'.

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'Virtual Boy (Beetle VB)'.

The content should now start running!

### Authors

- [Mednafen Team](https://mednafen.github.io/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

[GPLv2](https://github.com/libretro/beetle-vb-libretro/blob/master/COPYING)

## Extensions

Content that can be loaded by the Beetle VB core have the following file extensions:

- .vb
- .vboy
- .bin

## Databases

RetroArch database(s) that are associated with the Beetle VB core:

- [Nintendo - Virtual Boy](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Virtual%20Boy.rdb)

## Features

RetroArch-level settings or features that the Beetle VB core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
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
| Softpatching      | ✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✔         |

### Directories

The Beetle VB core's directory name is 'Mednafen VB'

The Beetle VB core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)
- 'content-name'.sav (Cartridge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The Beetle VB core's internal FPS is 50.27
- The Beetle VB core's internal sample rate is 44100 Hz
- The Beetle VB core's core provided aspect ratio is 12/7

## Core options

The Beetle VB core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Anaglyph preset (restart)** (**Off**/red & blue/red & cyan/red & electric cyan/red & green/green & magenta/yellow & blue)

<center> Select anaglyph 3D mode. </center>

!!! attention
	These Analglyph preset screenshots have been taken with the Palette core option set to black & red

??? note "Anaglyph preset - Off"
	![](images\Cores\beetle_vb\off.png)
	
??? note "Anaglyph preset - red & blue"
	![](images\Cores\beetle_vb\red&blue.png)

??? note "Anaglyph preset - red & cyan"
	![](images\Cores\beetle_vb\red&cyan.png)

??? note "Anaglyph preset - red & electric cyan"
	![](images\Cores\beetle_vb\red&electriccyan.png)

??? note "Anaglyph preset - red & green"
	![](images\Cores\beetle_vb\red&green.png)

??? note "Anaglyph preset - green & magenta"
	![](images\Cores\beetle_vb\green&magenta.png)

??? note "Anaglyph preset - yellow & blue"
	![](images\Cores\beetle_vb\yellow&blue.png)	

- **Palette (restart)** (**black & red**/black & white)

<center> Choose which color palette to use. </center>

??? note "Palette - black & red"
	![](images\Cores\beetle_vb\black&red.png)
	
??? note "Palette - black & white"
	![](images\Cores\beetle_vb\black&white.png)

## Controllers

### Device types

The Beetle VB core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- Retropad w/Analog - Joypad - There is no reason to switch to this.

### Controller tables

#### Joypad and analog device type table

| User 1 Input descriptors      | RetroPad Inputs                              |
|-------------------------------|----------------------------------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       |
| Select                        | ![](images/RetroPad/Retro_Select.png)        |
| Start                         | ![](images/RetroPad/Retro_Start.png)         |
| Left D-Pad Up                 | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| Left D-Pad Down               | ![](images/RetroPad/Retro_Dpad_Down.png)     | 
| Left D-Pad Left               | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| Left D-Pad Right              | ![](images/RetroPad/Retro_Dpad_Right.png)    |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       |
| L                             | ![](images/RetroPad/Retro_L1.png)            |
| R                             | ![](images/RetroPad/Retro_R1.png)            |
| Right D-Pad Up                | ![](images/RetroPad/Retro_L2.png)            |
| Right D-Pad Left              | ![](images/RetroPad/Retro_R2.png)            |
| Right D-Pad Down              | ![](images/RetroPad/Retro_L3.png)            |
| Right D-Pad Right             | ![](images/RetroPad/Retro_R3.png)            |

## Compatibility

Awaiting description.

## External Links

- [Libretro Beetle VB Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_vb_libretro.info)
- [Libretro Beetle VB Github Repository](https://github.com/libretro/beetle-vb-libretro)
- [Report Libretro Beetle VB Core Issues Here](https://github.com/libretro/beetle-vb-libretro/issues)
* [Official Website](https://mednafen.github.io/)
* [Official Upstream Downloads](https://mednafen.github.io/releases/)