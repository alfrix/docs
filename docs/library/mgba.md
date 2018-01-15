# Game Boy Advance (mGBA)

## Contribute to this documentation

**DOCUMENTATION IS A WORK IN PROGRESS**

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/mgba.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/meta/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

mGBA is an emulator for running Game Boy Advance games. It aims to be faster and more accurate than many existing Game Boy Advance emulators, as well as adding features that other emulators lack. It also supports Game Boy and Game Boy Color games.

### How to install the mGBA core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Game Boy Advance (mGBA)'.

<center> ![](images\Cores\updater\mgba.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start the mGBA core:

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

- If you are asked which core to select, choose 'Game Boy Advance (mGBA)'.

The content should now start running!

### Authors

- endrift

## See also

### GBA

- [Game Boy Advance (Beetle GBA)](https://docs.libretro.com/library/beetle_gba/)
- [Game Boy Advance (gpSP)](https://docs.libretro.com/library/gpsp/)
- [Game Boy Advance (Meteor)](https://docs.libretro.com/library/meteor/)
- [Game Boy Advance (VBA Next)](https://docs.libretro.com/library/vba_next/)
- [Game Boy Advance (VBA-M)](https://docs.libretro.com/library/vba_m/)

### GB/GBC

- [Game Boy / Game Boy Color (Emux GB)](https://docs.libretro.com/library/emux_gb/)
- [Game Boy / Game Boy Color (Gambatte)](https://docs.libretro.com/library/gambatte/)
- [Game Boy / Game Boy Color (SameBoy)](https://docs.libretro.com/library/sameboy/)
- [Game Boy / Game Boy Color (TGB Dual)](https://docs.libretro.com/library/tgb_dual/)
- [Game Boy / Game Boy Color (Gearboy)](https://docs.libretro.com/library/gearboy/)
- [SNES / Super Famicom (higan Accuracy)](https://docs.libretro.com/library/higan_accuracy/)
- [SNES / Super Famicom (nSide Balanced)](https://docs.libretro.com/library/nside_balanced/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The mGBA core is licensed under

- [MPLv2.0](https://github.com/libretro/mgba/blob/master/LICENSE)

## Extensions

Content that can be loaded by the mGBA core have the following file extensions:

- .gb
- .gbc
- .gba

## Databases

RetroArch database(s) that are associated with the mGBA core:

- [Nintendo - Game Boy](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy.rdb)
- [Nintendo - Game Boy Color](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Color.rdb)
- [Nintendo - Game Boy Advance](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Advance.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

|   Filename    |    Description                  |              md5sum              |
|:-------------:|:-------------------------------:|:--------------------------------:|
| gba_bios.bin  |Game Boy Advance BIOS - Optional | a860e8c0b6d573d191e4ec7db1b1e4f6 |

!!! warning
	In order for the Game Boy Advance BIOS to be used, the 'Use BIOS file if found' core option must be set to On.

## Features

RetroArch-level settings or features that the mGBA core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔ (not link-cable emulation) |
| Core Options      | ✔         |
| RetroAchievements | ✔ (GBA only) |
| RetroArch Cheats  | ✔         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | ✕         |
| Rumble            | ✔         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | ✔         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |
| LEDs              | ✕         |

### Directories

The mGBA core's directory name is 'mGBA'

The mGBA core saves/loads to/from these directories.

**RetroArch's Home directory**

- retroarch-core-options.cfg (Core-options)

**RetroArch's Config directory**

- mGBA.cfg (Core Overrides)
- 'content-name'.cfg (Game Overrides)
- 'content-name'.opt (Game-options)

**RetroArch's Input Remapping directory**

- mGBA.rmp (Core Remap)
- 'content-name'.rmp (Game Remap)

**RetroArch's Video Shader directory**

- mGBA.'shader-preset-extension' (Core Shader Preset)
- 'content-name'.'shader-preset-extension' (Game Shader Preset)

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'cotent-name'.state# (State)

### Geometry and timing

- The mGBA core's core provided FPS is (FPS)
- The mGBA core's core provided sample rate is 32768 Hz
- The mGBA core's core provided aspect ratio is (Ratio)

## Core options

The mGBA core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Solar sensor level** [mgba_solar_sensor_level] (0 to 10 in increments of 1. **0 is default.**)

	Can be used for games that employed the use of a solar sensor on their cartridges.
	
- **Allow opposing directional input** [mgba_allow_opposing_directions] (**Off**/On)

	Self-explanatory.
	
- **Use BIOS file if found** [mgba_use_bios] (Off/**On**)
	
	Uses a Game Boy Advance BIOS present in RetroArch's system directory. Look at the [BIOS section](file:///C:/rootw/Backup/port/git/docs/site/library/mgba/index.html#bios) for more information.
	
- **Skip BIOS intro** [mgba_skip_bios] (**Off**/On)
	
	Skips the BIOS intro when a Game Boy Advance BIOS present in RetroArch's system directory is used. The 'Use BIOS file if found' core option must be set to On for proper operation.

??? note "Skip BIOS intro - Off"
    ![](images\Cores\mgba\bios.png)	

- **Idle loop removal** [mgba_idle_optimization] (**Remove Known**/Detect and Remove/Don't Remove)

	Awaiting description.
	
- **Frameskip** [mgba_frameskip] (0 to 10 in increments of 1. **0 is default**)

	Choose how much frames should be skipped to improve performance at the expense of visual smoothness.

## Controllers

The mGBA core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There's no reason to switch to this.

### Rumble support

Rumble only works in the mGBA core when

- The content being ran has rumble support. (e.g. Cartridges with a Rumble Pak)
- The joypad input driver being used has rumble support. (e.g. Xinput)
- The joypad device being used has rumble support.

### Controller tables

#### Joypad

| User 1 Remap descriptors | RetroPad Inputs                              |
|--------------------------|----------------------------------------------|
| B                        | ![](images/RetroPad/Retro_B_Round.png)       |
| Turbo B                  | ![](images/RetroPad/Retro_Y_Round.png)       |
| Select                   | ![](images/RetroPad/Retro_Select.png)        |
| Start                    | ![](images/RetroPad/Retro_Start.png)         |
| Up                       | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| Down                     | ![](images/RetroPad/Retro_Dpad_Down.png)     |
| Left                     | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| Right                    | ![](images/RetroPad/Retro_Dpad_Right.png)    |
| A                        | ![](images/RetroPad/Retro_A_Round.png)       |
| Turbo A                  | ![](images/RetroPad/Retro_X_Round.png)       |
| L                        | ![](images/RetroPad/Retro_L1.png)            |
| R                        | ![](images/RetroPad/Retro_R1.png)            |
| Turbo L                  | ![](images/RetroPad/Retro_L2.png)            |
| Turbo R                  | ![](images/RetroPad/Retro_R2.png)            |
| Darken Solar Sensor      | ![](images/RetroPad/Retro_L3.png)            |
| Brighten Solar Sensor    | ![](images/RetroPad/Retro_R3.png)            |

## External Links

- [Official mGBA Website](https://mgba.io/)
- [Official mGBA Github Repository](https://github.com/mgba-emu/mgba)

- [Libretro mGBA Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mgba_libretro.info)
- [Libretro mGBA Github Repository](https://github.com/libretro/mgba)
- [Report Libretro mGBA Core Issues Here](https://github.com/mgba-emu/mgba/issues)