# Game Boy / Gameboy Color (Gearboy)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/gearboy.md). Changes are proposed using "Pull Requests."

There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)

You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).

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
- Saves battery powered RAM cartridges to file.

### How to get and install the Gearboy core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Game Boy / Gameboy Color (Gearboy)'.

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'Game Boy / Gameboy Color (Gearboy)'.

The content should now start running!

### Authors

- Ignacio Sanchez

## See also

- [Game Boy / Game Boy Color (Emux GB)](https://docs.libretro.com/library/emux_gb/)
- [Game Boy / Game Boy Color (Gambatte)](https://docs.libretro.com/library/gambatte/)
- [Game Boy / Game Boy Color (SameBoy)](https://docs.libretro.com/library/sameboy/)
- [Game Boy / Game Boy Color (TGB Dual)](https://docs.libretro.com/library/tgbdual/)
- [Game Boy Advance (mGBA)](https://docs.libretro.com/library/mgba/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

- [GPLv3](https://github.com/libretro/Gearboy/blob/master/LICENSE)

## Extensions

Content that can be loaded by the Gearboy core have the following file extensions:

- .gb
- .gbc

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
| Softpatching      | ✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The Gearboy core's directory name is 'Gearboy'

### Geometry and timing

- The Gearboy core's internal FPS is 59.727
- The Gearboy core's internal sample rate is 44100 Hz
- The Gearboy core's core provided aspect ratio is (Ratio)

## Controllers

### Device types

The Gearboy core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- Nintendo Gameboy - Joypad

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

- [Libretro Gearboy Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/gearboy_libretro.info)
- [Libretro Gearboy Github Repository](https://github.com/libretro/Gearboy)
- [Report Libretro Gearboy Core Issues Here](https://github.com/libretro/libretro-meta/issues)
- [Official Gearboy Github Repository](https://github.com/drhelius/Gearboy)
