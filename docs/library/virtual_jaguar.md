# Atari - Jaguar (Virtual Jaguar)

## Background

Virtual Jaguar is a portable Jaguar emulator which is based on the source code of what used to be Potato Emulation.

### Author/License

The Virtual Jaguar core has been authored by

- David Raingeard
- Shamus

The Virtual Jaguar core is licensed under

- [GPLv3](https://github.com/libretro/virtualjaguar-libretro/blob/master/docs/GPLv3)

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

## Extensions

Content that can be loaded by the Virtual Jaguar core have the following file extensions:

- .j64
- .jag
- .rom
- .abs
- .cof
- .bin
- .prg

## Databases

RetroArch database(s) that are associated with the Virtual Jaguar core:

- [Atari - Jaguar](https://github.com/libretro/libretro-database/blob/master/rdb/Atari%20-%20Jaguar.rdb)

## Features

Frontend-level settings or features that the Virtual Jaguar core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✕         |
| Rewind            | ✕         |
| Netplay           | ✕         |
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
| Crop Overscan     | ✕         |
| LEDs              | ✕         |

### Directories

The Virtual Jaguar core's internal core name is 'Virtual Jaguar'

The Virtual Jaguar core saves/loads to/from these directories.

-**Frontend's Home directory**

- cdrom.eeprom (Save)
- 'Game-CRC'.eeprom (Save)

### Geometry and timing

- The Virtual Jaguar core's core provided FPS is 50 for PAL games and 60 for NTSC games.
- The Virtual Jaguar core's core provided sample rate is 48000 Hz
- The Virtual Jaguar core's core provided aspect ratio is 4/3

## Core options

The Virtual Jaguar core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Fast Blitter** [virtualjaguar_usefastblitter] (**disabled**|enabled)

	This option will force Virtual Jaguar to use the older, less compatible yet faster blitter. Some games will not work properly with this option on.
	
- **Doom Res Hack** [virtualjaguar_doom_res_hack] (**disabled**|enabled)

	Needed for Doom to run in its correct resolution.
	
??? note "*Doom Res Hack - Disabled*"
    ![](images\Cores\virtual_jaguar\doom_off.png)

??? note "*Doom Res Hack - Enabled*"
    ![](images\Cores\virtual_jaguar\doom_on.png)
	
- **Bios** [virtualjaguar_bios] (**disabled**|enabled)

	Enables bios loading sequence.
	
??? note "*Bios - Enabled*"
    ![](images\Cores\virtual_jaguar\bios.png)
	
- **Pal (Restart)** [virtualjaguar_pal] (**disabled**|enabled)

	NTSC to PAL switch. Setting this to on switches to PAL mode.
	
## Controllers

The Virtual Jaguar core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 - 2 device types

![](images/Controllers/jaguar.png)

- None - Doesn't disable input. There's no reason to switch to this.
- **RetroPad** - Joypad - Stay on this.
- RetroPad w/Analog - Joypad - Same as RetroPad. There's no reason to switch to this.

### Controller tables

#### Joypad

| User 1 - 2 Remap descriptors | RetroPad Inputs                           |                       
|------------------------------|-------------------------------------------|
| B                            | ![](images/RetroPad/Retro_B_Round.png)    |
| C                            | ![](images/RetroPad/Retro_Y_Round.png)    |
| Pause                        | ![](images/RetroPad/Retro_Select.png)     |
| Option                       | ![](images/RetroPad/Retro_Start.png)      |
| D-Pad Up                     | ![](images/RetroPad/Retro_Dpad_Up.png)    |
| D-Pad Down                   | ![](images/RetroPad/Retro_Dpad_Down.png)  |
| D-Pad Left                   | ![](images/RetroPad/Retro_Dpad_Left.png)  |
| D-Pad Right                  | ![](images/RetroPad/Retro_Dpad_Right.png) |
| A                            | ![](images/RetroPad/Retro_A_Round.png)    |
| Numpad 0                     | ![](images/RetroPad/Retro_X_Round.png)    |
| Numpad 1                     | ![](images/RetroPad/Retro_L1.png)         |
| Numpad 2                     | ![](images/RetroPad/Retro_R1.png)         |
| Numpad 3                     | ![](images/RetroPad/Retro_L2.png)         |
| Numpad 4                     | ![](images/RetroPad/Retro_R2.png)         |
| Numpad 5                     | ![](images/RetroPad/Retro_L3.png)         |
| Numpad 6                     | ![](images/RetroPad/Retro_R3.png)         |

## Compatibility

A reference compatibility table can be found on the bottom of this [page](https://icculus.org/virtualjaguar/)

| Game           | Issue                                                   |
|----------------|---------------------------------------------------------|
| Cybermorph     | Graphics glitches. (1)                                  |
| Doom           | Enable Doom core option hack for proper graphics pitch. |
| Iron Soldier   | Hangs after selecting a stage.                          |
| Iron Soldier 2 | Hangs after selecting a stage. Audio glitches.          |
| Kasumi Ninja   | Graphics glitches. Missing background layers (2)        |
| Ruiner Pinball | Doesn't boot.                                           |
| Super Burnout  | Hangs after selecting a track.                          |
| Towers II      | Heavy flickering.                                       |
| Wolfenstein 3D | Doesn't boot.                                           |

??? note "(1)"
    ![](images\Cores\virtual_jaguar\cyber.png)

??? note "(2)"
    ![](images\Cores\virtual_jaguar\ninja.png)

## External Links

- [Official Virtual Jaguar Website](https://icculus.org/virtualjaguar/)
- [Official Virtual Jaguar Git Repository](http://shamusworld.gotdns.org/git/virtualjaguar)
- [Libretro Virtual Jaguar Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/virtualjaguar_libretro.info)
- [Libretro Virtual Jaguar Github Repository](https://github.com/libretro/virtualjaguar-libretro)
- [Report Libretro Virtual Jaguar Core Issues Here](https://github.com/libretro/virtualjaguar-libretro/issues)