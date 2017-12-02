# Sega MS/MD/CD/32X (PicoDrive)

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/picodrive.md). Changes are proposed using "Pull Requests."

## Background

PicoDrive is an open-source Sega 8/16 bit and 32X emulator which was written having ARM-based handheld devices in mind.

### Why use this core?

- Only libretro core that supports 32x emulation.

- If your preferred device is too weak to run any other cores.

### How to get and install the PicoDrive core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Sega MS/MD/CD/32X (PicoDrive)'.

After this has finished downloading, the core should now be ready for use!

### Authors

- notaz
- fdave

## See also

- [Sega Master System (Emux)](https://buildbot.libretro.com/docs/library/emux_sms/)
- [Sega MS/GG/MD/CD (Genesis Plus GX)](https://buildbot.libretro.com/docs/library/genesis_plus_gx/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://buildbot.libretro.com/docs/tech/licenses/).

- [MAME](https://github.com/libretro/picodrive/blob/master/COPYING)

## Extensions

Content that can be loaded by the PicoDrive core have the following file extensions:

- .bin
- .gen
- .smd
- .md
- .32x
- .cue
- .iso
- .sms
- .68k

## Databases

RetroArch database(s) that are associated with the PicoDrive core:

- [Sega - Master System - Mark III](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Master%20System%20-%20Mark%20III.rdb)
- [Sega - Mega Drive - Genesis](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Mega%20Drive%20-%20Genesis.rdb)
- [Sega - PICO](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20PICO.rdb)
- [Sega - 32X](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%2032X.rdb)

## BIOS

*Required or optional firmware files go in RetroArch's system directory.*

|   Filename    |    Description            |              md5sum              |
|:-------------:|:-------------------------:|:--------------------------------:|
| bios_CD_E.bin | MegaCD EU BIOS - Required | e66fa1dc5820d254611fdcdba0662372 |
| bios_CD_U.bin | SegaCD US BIOS - Required | 2efd74e3232ff260e371b99f84024f7f |
| bios_CD_J.bin | MegaCD JP BIOS - Required | 278a9397d192149e84e820ac621a8edd |

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| RetroAchievements | ✔         |
| RetroArch Cheats  | ✔         |
| Native Cheats     | ✕         |
| Controllers       | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| Softpatching      | ✕         |

### Saves/States

The PicoDrive core's directory name is 'PicoDrive'

Game data is saved/loaded to and from where save files are stored.

- .srm (Battery save)

Save states are saved/loaded to and from where state files are stored.

- .state (State)

## Core options

The PicoDrive core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.

- **Input device 1** (**3 button pad**/6 button pad/None): Choose which kind of controller is plugged in slot 1.
- **Input device 2** (**3 button pad**/6 button pad/None): Choose which kind of controller is plugged in slot 2.
- **No sprite limit** (**Off**/On): Enable this to remove the sprite limit.
- **MegaCD RAM cart** (**Off**/On): Emulate a MegaCD RAM cart.
- **Region** (**Auto**/Japan NTSC/Japan PAL/US/Europe): Force a specific region.
- **Core-provided aspect ratio** (**PAR**/ 4/3 /CRT): Choose the core-provided aspect ratio. RetroArch's aspect ratio must be set to Core provided in the Video seetings. 

??? note "Core-provided aspect ratio - PAR"
	![PAR](images\Cores\picodrive\PAR.png)
	
??? note "Core-provided aspect ratio - 4/3"
	![4by3](images\Cores\picodrive\4by3.png)

??? note "Core-provided aspect ratio - CRT"
	![CRT](images\Cores\picodrive\CRT.png)	

- **Show Overscan** (**Off**/On): Crop out the potentially random glitchy video output that would have been hidden by the bezel around the edge of a standard-definition television screen.

??? note "Show Overscan - Off"
	![overscan_off](images\Cores\picodrive\overscan_off.png)
	
??? note "Show Overscan - On"
	![overscan_on](images\Cores\picodrive\overscan_on.png)	

- **68k overclock** (**Off**/+25%/+50%/+75%/+100%/+200%/+400%): Overclock the emulated [68k chip](http://segaretro.org/M68000)

- **Dynamic recompilers** (Off/**On**): Enable dynamic recompilers which help to improve performance. **This core option is not available on all hardware.**

## Controllers

The PicoDrive core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 - 2 device types

- **RetroPad** - Joypad with analog
- RetroPad w/Analog - **There is no reason to switch to this.**

### Controllers graph

| PicoDrive   | RetroPad                                                       |
|-------------|----------------------------------------------------------------|
| B           | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               |
| A           | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)               |
| Mode        | ![RetroPad_Select](images/RetroPad/Retro_Select.png)           |
| Start       | ![RetroPad_Start](images/RetroPad/Retro_Start.png)             |
| D-Pad Up    | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            |
| D-Pad Down  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          |
| D-Pad Left  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          |
| D-Pad Right | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         |
| C           | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               |
| Y           | ![RetroPad_X](images/RetroPad/Retro_X_Round.png)               |
| X           | ![RetroPad_L1](images/RetroPad/Retro_L1.png)                   |
| Z           | ![RetroPad_R1](images/RetroPad/Retro_R1.png)                   |

## Compatibility

| 32x games                                    | Issue                                                         |
|----------------------------------------------|---------------------------------------------------------------|
| Brutal Unleashed – Above the Claw            | Softlocks after the first fight.                              |
| FIFA Soccer ’96                              | Glitched main menu text.                                      |
| Knuckles’ Chaotix                            | Glitched graphics on the Player Select screen.                |
| NBA Jam Tournament Edition                   | Framerate issues.                                             |
| NFL Quarterback Club                         | Some menu graphics are missing.                               |
| Star Wars Arcade (PAL version)               | Glitched opening visuals. Cannot get past Press Start screen. |
| Virtua Racing Deluxe                         | Blinking line during the SEGA logo screen.                    |
| World Series Baseball Starring Deion Sanders | Crashes when starting a match.                                |
| WWF Raw                                      | Various graphics are missing.                                 |

## External Links

- [Libretro PicoDrive Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/picodrive_libretro.info)
- [Libretro PicoDrive Github Repository](https://github.com/libretro/picodrive)
- [Report Libretro PicoDrive Core Issues Here](https://github.com/libretro/picodrive/issues)
* [Official Website](http://notaz.gp2x.de/pico.php)
* [Official Repository](https://github.com/notaz/picodrive)