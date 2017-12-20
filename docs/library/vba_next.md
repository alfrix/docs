# Game Boy Advance (VBA Next)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/vba_next.md). Changes are proposed using "Pull Requests."

There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)

## Background

VBA-Next is a Game Boy Advance emulator based on VBA-M 2011 with backported patches for performance and compatibility improvements.

### Why use this core?

Awaiting description.

### How to get and install the VBA Next core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Game Boy Advance (VBA Next)'.

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'Game Boy Advance (VBA Next)'.

The content should now start running!

### Authors

- Forgotten
- VBA-M Team
- Squarepusher

## See also

### GBA

- [Game Boy Advance (Beetle GBA)](https://docs.libretro.com/library/beetle_gba/)
- [Game Boy Advance (gpSP)](https://docs.libretro.com/library/gpsp/)
- [Game Boy Advance (Meteor)](https://docs.libretro.com/library/meteor/)
- [Game Boy Advance (mGBA)](https://docs.libretro.com/library/mgba/)
- [Game Boy Advance (VBA Next)](https://docs.libretro.com/library/vba_next/)
- [Game Boy Advance (VBA-M)](https://docs.libretro.com/library/vbam/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

- GPLv2

## Extensions

Content that can be loaded by the VBA Next core have the following file extensions:

- .gba

## Databases

RetroArch database(s) that are associated with the VBA Next core:

- [Nintendo - Game Boy Advance](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Advance.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

|   Filename    |    Description                    |              md5sum              |
|:-------------:|:---------------------------------:|:--------------------------------:|
| gba_bios.bin  | Game Boy Advance Image - Optional | a860e8c0b6d573d191e4ec7db1b1e4f6 |

!!! warning
	In order for the Game Boy Advance BIOS to be used, the 'Use bios if available' core option must be set to On.
	
## Features

RetroArch features that the VBA Next core respects.

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

The VBA Next core's directory name is 'VBA Next'

The VBA Next core loads from and saves to to these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'content-name-.state# (State)

### Geometry and timing

The VBA Next core's internal FPS is 59.7275005696.

The VBA Next core's internal sample rate is 32000 Hz

The VBA Next core's core provided aspect ratio is 3/2

## Core options

The VBA Next core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Use bios if available (Restart)** (Off/**On**)

<center> Self-explanatory. Look at the [BIOS section](https://docs.libretro.com/library/vba_next/#bios) for more information. </center>

??? note "Use bios if available - On"
	![](images\Cores\vba_next\bios.png)

## Controllers

### Device types

The VBA Next core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - **There is no reason to switch to this**.

### Controller tables

#### Joypad and analog device type table

| User 1 input descriptors      | RetroPad Inputs                              | RetroPad           |
|-------------------------------|----------------------------------------------|--------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                  |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select             |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start              |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up           |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down         |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left         |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right        |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | A                  |
| L                             | ![](images/RetroPad/Retro_L1.png)            | L                  |
| R                             | ![](images/RetroPad/Retro_R1.png)            | R                  |

## Compatibility

| Game                                  | Issue                          |
|---------------------------------------|--------------------------------|
|**Advanced Dungeons & Dragons - Deathkeep**| Random softlocks (music related?). |
|**Alone in the Dark**|Unreadable text within books. Audio glitches. |
|**DinoPark Tycoon**| 	Graphics glitches. |
|**Eye of Typhoon, The**| 	Runs too fast. |
|**Horde, The**| 	Graphics glitches. Minor graphical inaccuracy in bird's eye map. |
|**Primal Rage**|Primal Rage|
|**Psychic Detective**|Psychic Detective|
|**Psychic Detective**|Psychic Detective|
|**Tetsujin Return**| 	Graphics glitches. Missing graphics for obstacles in the driving scenes. |

## External Links

- [Libretro VBA Next Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/vba_next_libretro.info)
- [Libretro VBA Next Github Repository](https://github.com/libretro/vba-next)
- [Report Libretro VBA Next Core Issues Here](https://github.com/libretro/vba-next/issues)