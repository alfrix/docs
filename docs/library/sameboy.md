# Game Boy/Game Boy Color (SameBoy)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/sameboy.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

SameBoy is an extremely accurate open source Gameboy (DMG) and Gameboy Color (CGB) emulator, written in portable C.

### Why use this core?

- Supports GameBoy (DMG) and GameBoy Color (CGB) emulation
- Battery save support
- Save states
- Includes open source DMG and CGB boot ROMs
- Real time clock emulation
- Extremely high accuracy

### How to get and install the SameBoy core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Game Boy/Game Boy Color (SameBoy)'.

<center> ![](images\Cores\sameboy\sameboy.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\gb.png) </center>

- If you are asked which core to select, choose 'Game Boy/Game Boy Color (SameBoy)'.

The content should now start running!

### Authors

- LIJI32

## See also

### GB/GBC

- [Game Boy / Game Boy Color (Emux GB)](https://docs.libretro.com/library/emux_gb/)
- [Game Boy / Game Boy Color (Gambatte)](https://docs.libretro.com/library/gambatte/)
- [Game Boy / Game Boy Color (TGB Dual)](https://docs.libretro.com/library/tgb_dual/)
- [Game Boy / Game Boy Color (Gearboy)](https://docs.libretro.com/library/gearboy/)
- [Game Boy Advance (mGBA)](https://docs.libretro.com/library/mgba/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The SameBoy core is licensed under

- [MIT](https://github.com/libretro/SameBoy/blob/master/LICENSE)

## Extensions

Content that can be loaded by the SameBoy core have the following file extensions:

- .gb
- .gbc

## Databases

RetroArch database(s) that are associated with the SameBoy core:

- [Nintendo - Game Boy](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy.rdb)
- [Nintendo - Game Boy Color](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Color.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

!!! attention
	The SameBoy core has reverse engineered Game Boy/Game Boy Color boot ROMs baked into the core itself so real BIOS files aren't required. If you’d like to override this, you can place the following BIOS files in RetroArch's system directory.

|   Filename   |      Description                   |              md5sum              |
|:------------:|:----------------------------------:|:--------------------------------:|
| dmg_boot.bin | Game Boy boot ROM - Optional       | 32fbbd84168d3482956eb3c5051637f5 |
| cgb_boot.bin | Game Boy Color boot ROM - Optional | dbfce9db9deaa2567f6a84fde55f9680 |

## Features

RetroArch-level settings or features that the SameBoy core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔ (not link-cable emulation) |
| Core Options      | ✔         |
| RetroAchievements | ✔         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | ✕         |
| Rumble            | ✔         |
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

The SameBoy core's directory name is 'SameBoy'

The SameBoy core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge backup save)
- 'content-name'.rtc (Real time clock save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The SameBoy core's internal FPS is 59.72
- The SameBoy core's internal sample rate is 44100 Hz
- The SameBoy core's core provided aspect ratio is 160/144

## Core options

The SameBoy core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with SameBoy means that core has to be closed for the new setting to be applied on next launch.

- **Color Correction** (**off**/correct curves/emulate hardware/preserve brightness)

<center> Self-explanatory. **Only for Gameboy Color games** </center>

??? note "Color Correction - off"
	![](images\Cores\sameboy\color_off.png)
	
??? note "Color Correction - correct curves"
	![](images\Cores\sameboy\color_curves.png)

??? note "Color Correction - emulate hardware"
	![](images\Cores\sameboy\color_hardware.png)

??? note "Color Correction - preserve brightness"
	![](images\Cores\sameboy\color_brightness.png)

- **High Pass Filter** (**off**/accurate/remove dc offset)

<center> Awaiting description. </center>

## Controllers

### Device types

The SameBoy core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- Nintendo Gameboy - Joypad

### Rumble support

Rumble only works in the SameBoy core when

- The content being ran has rumble support.
- The joypad input driver being used has rumble support. (e.g. Xinput)
- The joypad device being used has rumble support.

### Controller tables

#### Joypad and analog device type table

| User 1 Input descriptors      | RetroPad Inputs                              | Nintendo Gameboy   |
|-------------------------------|----------------------------------------------|--------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                  |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select             |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start              |
| Up                            | ![](images/RetroPad/Retro_Dpad_Up.png)       | Up                 |
| Down                          | ![](images/RetroPad/Retro_Dpad_Down.png)     | Down               |
| Left                          | ![](images/RetroPad/Retro_Dpad_Left.png)     | Left               |
| Right                         | ![](images/RetroPad/Retro_Dpad_Right.png)    | Right              |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | A                  |

## Compatibility

Awaiting description.

## External Links

- [Libretro SameBoy Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/sameboy_libretro.info)
- [Libretro SameBoy Github Repository](https://github.com/libretro/SameBoy)
- [Report Libretro SameBoy Core Issues Here](https://github.com/libretro/libretro-meta/issues)
- [Official SameBoy Website](https://sameboy.github.io/)
- [Official SameBoy Github Repository](https://github.com/LIJI32/SameBoy)