# Game Boy / Game Boy Color (Gearboy)

## Contribute to this documentation

**DOCUMENTATION IS A WORK IN PROGRESS**

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/gearboy.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Gearboy is a Nintendo Game Boy / GameBoy Color emulator written in C++.

### Why use this core?

- Highly accurate CPU emulation, passes cpu_instrs.gb from blargg's tests.
- Accurate instruction and memory timing, passes instr_timing.gb and mem_timing.gb from blargg's tests.
- Memory Bank Controllers (MBC1, MBC2, MBC3 with RTC, MBC5), ROM + RAM and multicart cartridges.
- Accurate LCD controller emulation. Background, window and sprites, with correct timings and priorities including mid-scanline timing.
- Mix frames: Mimics the LCD ghosting effect seen in the original Game Boy.
- Sound emulation using SDL Audio and Gb_Snd_Emu library.
- Game Boy Color support.
- Integrated disassembler. It can dump the full disassembled memory to a text file or access it in real time.
- Saves battery powered RAM cartridges to file.
- Compressed rom support (ZIP deflate).
- Multi platform. Runs on Windows, Linux, Mac OS X, Raspberry Pi and iOS.

### How to install the Gearboy core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Game Boy / Game Boy Color (Gearboy)'.

<center> ![](images\Cores\updater\gearboy.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start the Gearboy core:

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

- If you are asked which core to select, choose 'Game Boy / Game Boy Color (Gearboy)'.

The content should now start running!

### Authors

- Ignacio Sanchez

## See also

### GB/GBC

- [Game Boy / Game Boy Color (Emux GB)](https://docs.libretro.com/library/emux_gb/)
- [Game Boy / Game Boy Color (Gambatte)](https://docs.libretro.com/library/gambatte/)
- [Game Boy / Game Boy Color (SameBoy)](https://docs.libretro.com/library/sameboy/)
- [Game Boy / Game Boy Color (TGB Dual)](https://docs.libretro.com/library/tgb_dual/)
- [Game Boy Advance (mGBA)](https://docs.libretro.com/library/mgba/)
- [SNES / Super Famicom (higan Accuracy)](https://docs.libretro.com/library/higan_accuracy/)
- [SNES / Super Famicom (nSide Balanced)](https://docs.libretro.com/library/nside_balanced/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Gearboy core is licensed under

- [GPLv3](https://github.com/libretro/Gearboy/blob/master/LICENSE)

## Extensions

Content that can be loaded by the Gearboy core have the following file extensions:

- .gb
- .dmg
- .gbc
- .cgb
- .sgb

## Databases

RetroArch database(s) that are associated with the Gearboy core:

- [Nintendo - Game Boy](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy.rdb)
- [Nintendo - Game Boy Color](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Color.rdb)

## Features

RetroArch-level settings or features that the Gearboy core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✕         |
| Screenshots       | ✔         |
| Saves             | ✕         |
| States            | ✕         |
| Rewind            | ✕         |
| Netplay           | ✕         |
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
| [Softpatching](https://docs.libretro.com/guides/softpatching/) |✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |
| LEDs              | ✕         |

### Directories

The Gearboy core's directory name is 'Gearboy'

The Gearboy core saves/loads to/from these directories.

**RetroArch's Config directory**

- Gearboy.cfg (Core Overrides)
- 'content-name'.cfg (Game Overrides)
- 'content-name'.opt (Game-options)

**RetroArch's Input Remapping directory**

- Gearboy.rmp (Core Remap)
- 'content-name'.rmp (Game Remap)

**RetroArch's Video Shader directory**

- Gearboy.'shader-preset-extension' (Core Shader Preset)
- 'content-name'.'shader-preset-extension' (Game Shader Preset)

### Geometry and timing

- The Gearboy core's core provided FPS is 59.727
- The Gearboy core's core provided sample rate is 44100 Hz
- The Gearboy core's core provided aspect ratio is (Ratio)

## Controllers

The Gearboy core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- Nintendo Gameboy - Joypad

### Controller tables

#### Joypad

| User 1 Remap descriptors for 'Nintendo Gameboy' device type | RetroPad Inputs                              |
|-------------------------------------------------------------|----------------------------------------------|
| B                                                           | ![](images/RetroPad/Retro_B_Round.png)       |
| Select                                                      | ![](images/RetroPad/Retro_Select.png)        |
| Start                                                       | ![](images/RetroPad/Retro_Start.png)         |
| Up                                                          | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| Down                                                        | ![](images/RetroPad/Retro_Dpad_Down.png)     |
| Left                                                        | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| Right                                                       | ![](images/RetroPad/Retro_Dpad_Right.png)    |
| A                                                           | ![](images/RetroPad/Retro_A_Round.png)       |

## Compatibility

Awaiting description.

## External Links

- [Libretro Gearboy Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/gearboy_libretro.info)
- [Libretro Gearboy Github Repository](https://github.com/libretro/Gearboy)
- [Report Libretro Gearboy Core Issues Here](https://github.com/libretro/libretro-meta/issues)
- [Official Gearboy Github Repository](https://github.com/drhelius/Gearboy)