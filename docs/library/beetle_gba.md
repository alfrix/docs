# Nintendo - Game Boy Advance (Beetle GBA)

## Background

Standalone port of Mednafen GBA to libretro, itself a fork of VBA-M, itself a fork of Visual Boy Advance.

### Author/License

The Beetle GBA core has been authored by

- Forgotten
- [Mednafen Team](https://mednafen.github.io/)

The Beetle GBA core is licensed under

- [GPLv2](https://github.com/libretro/beetle-gba-libretro/blob/master/COPYING)

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

## Extensions

Content that can be loaded by the Beetle GBA core have the following file extensions:

- .gba
- .agb
- .bin

## Databases

RetroArch database(s) that are associated with the Beetle GBA core:

- [Nintendo - Game Boy Advance](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Advance.rdb)

## BIOS

Required or optional firmware files go in the frontend's system directory.

|   Filename   |    Description                   |              md5sum              |
|:------------:|:--------------------------------:|:--------------------------------:|
| gba_bios.bin | Game Boy Advance BIOS - Optional | a860e8c0b6d573d191e4ec7db1b1e4f6 |

## Features

Frontend-level settings or features that the Beetle GBA core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔ (not link-cable emulation)         |
| Core Options      | ✔         |
| RetroAchievements | ✔         |
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
| LEDs              | ✕         |

### Directories

The Beetle GBA core's internal core name is 'Mednafen VBA-M'

The Beetle GBA core saves/loads to/from these directories.

**Frontend's Save directory**

- 'content-name'.'ROM MD5'.sav (SRAM)
- 'content-name'.'ROM MD5'.eep (EEPROM)

**Frontend's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The Beetle GBA core's core provided FPS is 59.73
- The Beetle GBA core's core provided sample rate is 44100 Hz
- The Beetle GBA core's core provided aspect ratio is 3/2

## Core options

The Beetle GBA core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **HLE bios emulation** [gba_hle] (**enabled**/disabled)

	Self-explanatory. When set to off, a Game Boy Advance BIOS is required.

## Controllers

The Beetle GBA core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There's no reason to switch to this.

### Controller tables

#### Joypad

![](images/Controllers/gba.png)

| User 1 Remap descriptors | RetroPad Inputs                              |
|--------------------------|----------------------------------------------|
| B                        | ![](images/RetroPad/Retro_B_Round.png)       |
| Select                   | ![](images/RetroPad/Retro_Select.png)        |
| Start                    | ![](images/RetroPad/Retro_Start.png)         |
| D-Pad Up                 | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| D-Pad Down               | ![](images/RetroPad/Retro_Dpad_Down.png)     |
| D-Pad Left               | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| D-Pad Right              | ![](images/RetroPad/Retro_Dpad_Right.png)    |
| A                        | ![](images/RetroPad/Retro_A_Round.png)       |
| L                        | ![](images/RetroPad/Retro_L1.png)            | 
| R                        | ![](images/RetroPad/Retro_R1.png)            |

## External Links

- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)
- [Libretro Beetle GBA Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_gba_libretro.info)
- [Libretro Beetle GBA Github Repository](https://github.com/libretro/beetle-gba-libretro)
- [Report Libretro Beetle GBA Core Issues Here](https://github.com/libretro/beetle-gba-libretro/issues)

### See also

#### Nintendo - Game Boy Advance

- [Nintendo - Game Boy Advance (gpSP)](https://docs.libretro.com/library/gpsp/)
- [Nintendo - Game Boy Advance (Meteor)](https://docs.libretro.com/library/meteor/)
- [Nintendo - Game Boy Advance (mGBA)](https://docs.libretro.com/library/mgba/)
- [Nintendo - Game Boy Advance (TempGBA)](https://docs.libretro.com/library/tempgba/)
- [Nintendo - Game Boy Advance (VBA-M)](https://docs.libretro.com/library/vba_m/)
- [Nintendo - Game Boy Advance (VBA Next)](https://docs.libretro.com/library/vba_next/)