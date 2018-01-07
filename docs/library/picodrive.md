# Sega MS/MD/CD/32X (PicoDrive)

## Contribute to this documentation

**DOCUMENTATION IS A WORK IN PROGRESS**

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/picodrive.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

PicoDrive is an open-source Sega 8/16 bit and 32X emulator which was written having ARM-based handheld devices in mind.

### Why use this core?

- Only libretro core that supports 32x emulation.
- If your preferred device is too weak to run any other cores.

### How to install the PicoDrive core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Sega MS/MD/CD/32X (PicoDrive)'.

<center> ![](images\Cores\updater\picodrive.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start the PicoDrive core:

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

- If you are asked which core to select, choose 'Sega MS/MD/CD/32X (PicoDrive)'.

The content should now start running!

### Authors

- notaz
- fdave

## See also

### Sega 16-bit

- [Sega Master System (Emux SMS)](https://docs.libretro.com/library/emux_sms/)
- [Sega MS/GG/MD/CD (Genesis Plus GX)](https://docs.libretro.com/library/genesis_plus_gx/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The PicoDrive core is licensed under

- [Non-commercial](https://github.com/libretro/picodrive/blob/master/COPYING)

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

Required or optional firmware files go in RetroArch's system directory.

|   Filename    |    Description            |              md5sum              |
|:-------------:|:-------------------------:|:--------------------------------:|
| bios_CD_E.bin | MegaCD EU BIOS - Required | e66fa1dc5820d254611fdcdba0662372 |
| bios_CD_U.bin | SegaCD US BIOS - Required | 2efd74e3232ff260e371b99f84024f7f |
| bios_CD_J.bin | MegaCD JP BIOS - Required | 278a9397d192149e84e820ac621a8edd |

## Features

RetroArch-level settings or features that the PicoDrive core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
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
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | ✕         |
| Disk Control      | ✔         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |
| LEDs              | ✕         |

### Directories

The PicoDrive core's directory name is 'PicoDrive'

The PicoDrive core saves/loads to/from these directories.

**RetroArch's Config directory**

- PicoDrive.cfg (Core Overrides)
- 'content-name'.cfg (Game Overrides)
- 'content-name'.opt (Game-options)

**RetroArch's Input Remapping directory**

- PicoDrive.rmp (Core Remap)
- 'content-name'.rmp (Game Remap)

**RetroArch's Video Shader directory**

- PicoDrive.'shader-preset-extension' (Core Shader Preset)
- 'content-name'.'shader-preset-extension' (Game Shader Preset)

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge backup save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The PicoDrive core's core provided FPS is 60 for NTSC games and 50 for PAL games.
- The PicoDrive core's core provided sample rate is 44100 Hz
- The PicoDrive core's core provided aspect ratio is dependent on the ['Core-provided aspect ratio' core option](https://docs.libretro.com/picodrive/#core-options).

### Loading Sega CD content

PicoDrive needs a cue-sheet that points to an image file. A cue sheet, or cue file, is a metadata file which describes how the tracks of a CD or DVD are laid out.

If you have e.g. `foo.bin`, you should create a text file and save it as `foo.cue`. If you're playing a single-track Sega CD game, then the cue file contents should look like this:

`foobin.cue`
```
 FILE "foo.bin" BINARY
  TRACK 01 MODE1/2352
   INDEX 01 00:00:00
```

After that, you can load the `foo.cue` file in RetroArch with the PicoDrive core.

!!! attention
    Certain Sega CD games are multi-track, so their .cue files might be more complicated.

## Multiple-disk games

If foo is a multiple-disk game, you should have .cue files for each one, e.g. `foo (Disc 1).cue`, `foo (Disc 2).cue`, `foo (Disc 3).cue`.

To take advantage of PicoDrive's Disk Control feature for disk swapping, an index file (a m3u file) should be made.

Create a text file and save it as `foo.m3u`. Then enter your game's .cue files on it. The m3u file contents should look something like this:

`foo.m3u`
```
foo (Disc 1).cue
foo (Disc 2).cue
foo (Disc 3).cue
```

After that, you can load the `foo.m3u` file in RetroArch with the PicoDrive core.

## Core options

The PicoDrive core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Input device 1** (**3 button pad**/6 button pad/None)

	Choose which kind of controller is plugged in slot 1.
	
- **Input device 2** (**3 button pad**/6 button pad/None)

	Choose which kind of controller is plugged in slot 2.

- **No sprite limit** (**Off**/On)

	Enable this to remove the sprite limit.

- **MegaCD RAM cart** (**Off**/On)

	Emulate a MegaCD RAM cart.

- **Region** (**Auto**/Japan NTSC/Japan PAL/US/Europe)

	Force a specific region.

- **Core-provided aspect ratio** (**PAR**/ 4/3 /CRT)

	Choose the core-provided aspect ratio. RetroArch's aspect ratio must be set to Core provided in the Video seetings. 

??? note "Core-provided aspect ratio - PAR"
	![](images\Cores\picodrive\par.png)
	
??? note "Core-provided aspect ratio - 4/3"
	![](images\Cores\picodrive\4by3.png)

??? note "Core-provided aspect ratio - CRT"
	![](images\Cores\picodrive\crt.png)	

- **Show Overscan** (**Off**/On)

	Crop out the potentially random glitchy video output that would have been hidden by the bezel around the edge of a standard-definition television screen.

??? note "Show Overscan - Off"
	![](images\Cores\picodrive\overscan_off.png)
	
??? note "Show Overscan - On"
	![](images\Cores\picodrive\overscan_on.png)	

- **68k overclock** (**Off**/+25%/+50%/+75%/+100%/+200%/+400%)

	Overclock the emulated [68k chip](http://segaretro.org/M68000)

- **Dynamic recompilers** (Off/**On**)

	Enable dynamic recompilers which help to improve performance. **This core option is not available on all hardware.**

## Controllers

The PicoDrive core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 - 2 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog  - Joypad - There's no reason to switch to this.

### Controller tables

#### Joypad

| User 1 - 2 Remap descriptors | RetroPad Inputs                              | 3 button pad  | 6 button pad |
|------------------------------|----------------------------------------------|---------------|--------------|
| B                            | ![](images/RetroPad/Retro_B_Round.png)       | B             | B            |
| A                            | ![](images/RetroPad/Retro_Y_Round.png)       | A             | A            |
| Mode                         | ![](images/RetroPad/Retro_Select.png)        |               | Mode         |
| Start                        | ![](images/RetroPad/Retro_Start.png)         | Start         | Start        |
| D-Pad Up                     | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up      | D-Pad Up     |
| D-Pad Down                   | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down    | D-Pad Down   |
| D-Pad Left                   | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left    | D-Pad Left   |
| D-Pad Right                  | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right   | D-Pad Right  |
| C                            | ![](images/RetroPad/Retro_A_Round.png)       | C             | C            |
| Y                            | ![](images/RetroPad/Retro_X_Round.png)       |               | Y            |
| X                            | ![](images/RetroPad/Retro_L1.png)            |               | X            |
| Z                            | ![](images/RetroPad/Retro_R1.png)            |               | Z            |

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
- [Official PicoDrive Website](http://notaz.gp2x.de/pico.php)
- [Official PicoDrive Github Repository](https://github.com/notaz/picodrive)