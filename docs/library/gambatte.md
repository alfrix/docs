# Game Boy / Game Boy Color (Gambatte)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/gambatte.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Gambatte is an accuracy-focused, open-source, cross-platform Game Boy Color emulator written in C++. It is based on hundreds of corner case hardware tests, as well as previous documentation and reverse engineering efforts.

### Why use this core?

Awaiting description.

### How to get and install the Gambatte core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Game Boy / Game Boy Color (Gambatte)'.

<center> ![](images\Cores\gambatte\gambatte.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\gb.png) </center>

- If you are asked which core to select, choose 'Game Boy / Game Boy Color (Gambatte)'.

The content should now start running!

### Authors

- Sinamas

## See also

### GB/GBC

- [Game Boy / Game Boy Color (Emux GB)](https://docs.libretro.com/library/emux_gb/)
- [Game Boy / Game Boy Color (SameBoy)](https://docs.libretro.com/library/sameboy/)
- [Game Boy / Game Boy Color (TGB Dual)](https://docs.libretro.com/library/tgb_dual/)
- [Game Boy / Game Boy Color (Gearboy)](https://docs.libretro.com/library/gearboy/)
- [Game Boy Advance (mGBA)](https://docs.libretro.com/library/mgba/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Gambatte core is licensed under

- [GPLv2](https://github.com/libretro/gambatte-libretro/blob/master/COPYING)

## Extensions

Content that can be loaded by the Gambatte core have the following file extensions:

- .gb
- .gbc
- .dmg

## Databases

RetroArch database(s) that are associated with the Gambatte core:

- [Nintendo - Game Boy](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy.rdb)
- [Nintendo - Game Boy Color](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Color.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

|   Filename     |    Description                 |              md5sum              |
|:--------------:|:------------------------------:|:--------------------------------:|
| gb_bios.bin    | Game Boy BIOS - Optional       | 32fbbd84168d3482956eb3c5051637f5 |
| gbc_bios.bin   | Game Boy Color BIOS - Optional | dbfce9db9deaa2567f6a84fde55f9680 |

!!! attention
	The ['Use official bootloader' core option](https://docs.libretro.com/library/gambatte#core-options) must be set to On in order for these BIOS files to be used.

## Features

RetroArch-level settings or features that the Gambatte core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✕         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔          |
| Netplay           | ✔ (not link-cable emulation) |
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

The Gambatte core's directory name is 'Gambatte'

The Gambatte core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The Gambatte core's internal FPS is (FPS)
- The Gambatte core's internal sample rate is (Rate)
- The Gambatte core's core provided aspect ratio is (Ratio)

## Custom palettes for Game Boy games

The GB Colorization core option must be set to custom.

Create a folder called "palettes" in RetroArch's system directory. Then, you can place custom palette files (.pal) inside the "palettes" folder

You can define different palettes for specific games by creating a .pal file in the "palettes" folder with "INTERNALROMNAME.pal" or "rom-name.pal". If no specific palette is found for a ROM then the default palette is used.

You can also define a palette to be used for all Game Boy games by creating a .pal file in the "palettes" folder named "Default.pal"

??? note "*Custom palettes can be created from the GUI in standalone Gambatte*"
    ![](images\Cores\gambatte\tool.png)

## Core options

The Gambatte core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **GB Colorization** (**Off**/auto/internal/custom)

<center> Colorizes Game Boy games. </center>

??? note "*GB Colorization - Off*"
    ![](images\Cores\gambatte\color_off.png)

??? note "*GB Colorization - auto*"
    ![](images\Cores\gambatte\color_auto.png)

- **Internal Palette** (**GBC - Blue**/GBC - Brown/GBC - Dark Blue/GBC - Dark Brown/GBC - Dark Green/GBC - Grayscale/GBC - Green/GBC - Inverted/GBC - Orange/GBC - Pastel Mix/GBC - Red/GBC - Yellow/Special 1/Special 2/Special 3)

<center> Select which internal color palette for GB Colorization is going to be used. GB Colorization must be set to internal. </center>

??? note "*Internal Palette - GBC - Blue*"
    ![](images\Cores\gambatte\blue.png)

??? note "*Internal Palette - GBC - Brown*"
    ![](images\Cores\gambatte\brown.png)

??? note "*Internal Palette - GBC - Dark Blue*"
    ![](images\Cores\gambatte\dark_blue.png)

??? note "*Internal Palette - GBC - Dark Brown*"
    ![](images\Cores\gambatte\dark_brown.png)

??? note "*Internal Palette - GBC - Dark Green*"
    ![](images\Cores\gambatte\dark_green.png)

??? note "*Internal Palette - GBC - Grayscale*"
    ![](images\Cores\gambatte\grayscale.png)

??? note "*Internal Palette - GBC - Green*"
    ![](images\Cores\gambatte\green.png)

??? note "*Internal Palette - GBC - Inverted*"
    ![](images\Cores\gambatte\inverted.png)

??? note "*Internal Palette - GBC - Orange*"
    ![](images\Cores\gambatte\orange.png)

??? note "*Internal Palette - GBC - Pastel Mix*"
    ![](images\Cores\gambatte\pastel.png)

??? note "*Internal Palette - GBC - Red*"
    ![](images\Cores\gambatte\red.png)

??? note "*Internal Palette - GBC - Yellow*"
    ![](images\Cores\gambatte\yellow.png)

??? note "*Internal Palette - GBC - Special 1*"
    ![](images\Cores\gambatte\special1.png)

??? note "*Internal Palette - GBC - Special 2*"
    ![](images\Cores\gambatte\special2.png)

??? note "*Internal Palette - GBC - Special 3*"
    ![](images\Cores\gambatte\special3.png)

- **Color Correction** (**On**/Off)

<center> Darkens Game Boy Color games to match the original hardware output. </center>

??? note "*Color Correction - On*"
    ![](images\Cores\gambatte\correct_on.png)

??? note "*Color Correction - Off*"
    ![](images\Cores\gambatte\correct_off.png)

- **Emulated Hardware (restart)** (**Auto**/GB/GBC/GBA)

<center> Choose which hardware is emulated Game Boy, Game Boy Color, or Game Boy Advance. </center>

- **Use official bootloader (restart) (if available)** (**On**/Off)

<center> Enables support for using official Game Boy and Game Boy Color bootloaders with startup logos. Check the [BIOS section](https://docs.libretro.com/library/gambatte#bios) to see what files are needed. </center>

??? note "*Game Boy bootloader*"
    ![](images\Cores\gambatte\gb_bios.png)

??? note "*Game Boy Color bootloader*"
    ![](images\Cores\gambatte\gbc_bios.png)

- **Gameboy Link Mode:** (**Not Connected**/Network Server/Network Client)

<center> Awaiting description. </center>

- **Network Link Port:** (**56400**-56420)

<center> Awaiting description. </center>

- **Network link server add:** (**0**-255)

<center> Awaiting description. </center>

- **Network link server add:** (**0**-255)

<center> Awaiting description. </center>

- **Network link server add:** (**0**-255)

<center> Awaiting description. </center>

- **Network link server add:** (**0**-255)

<center> Awaiting description. </center>

## Controllers

### Device types

The Gambatte core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad

### Controller tables

#### Joypad and analog device type table

| User 1 Input descriptors      | RetroPad Inputs                              |
|-------------------------------|----------------------------------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       |
| Select                        | ![](images/RetroPad/Retro_Select.png)        |
| Start                         | ![](images/RetroPad/Retro_Start.png)         |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       |

## Compatibility

| Game                                              | Issue                                              |
|---------------------------------------------------|----------------------------------------------------|
| Command Master                                    | Crashes on start. Unemulated MBC7 mapper.          |
| Game Boy Camera                                   | Crashes on start. Unemulated Pocket Camera mapper. |
| Game de Hakken!! Tamagotchi - Osutchi to Mesutchi | Crashes on start. Unemulated TAMA5 mapper.         |
| Kirby Tilt 'n' Tumble                             | Crashes on start. Unemulated MBC7 mapper.          |
| Net de Get: Mini-Game @ 100                       | Crashes on start. Unemulated MBC6 mapper.          |
| Pocket Family GB2                                 | Crashes on start. Unemulated HuC3 mapper.          |
| Robopon: Sun/Star/Moon Version                    | Crashes on start. Unemulated HuC3 mapper.          |

## External Links

- [Libretro Gambatte Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/gambatte_libretro.info)
- [Libretro Gambatte Github Repository](https://github.com/libretro/gambatte-libretro)
- [Report Libretro Gambatte Core Issues Here](https://github.com/libretro/gambatte-libretro/issues)
- [Official Gambatte Github Repository](https://github.com/sinamas/gambatte)
- [Old Standalone Gambatte builds](https://sourceforge.net/projects/gambatte/files/gambatte/)