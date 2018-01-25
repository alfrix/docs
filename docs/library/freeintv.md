# Mattel - Intellivision (FreeIntv)

## Contribute to this documentation

**DOCUMENTATION IS A WORK IN PROGRESS**

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/freeintv.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/meta/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

FreeIntv is a libretro emulation core for the Mattel Intellivision designed to be compatible with joypads from the SNES era forward even if they originally required a number pad.

**Note: FreeIntv does not currently emulate Entertainment Computer System (ECS) and Intellivoice functionality. Contributions to the source are welcome!**


### How to install the FreeIntv core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info Files'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Mattel - Intellivision (FreeIntv)'.

<center> ![](images\Cores\updater\screenshot_name.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start the FreeIntv core:

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

- If you are asked which core to select, choose 'Mattel - Intellivision (FreeIntv)'.

The content should now start running!

### Authors

- FreeIntv was created by David Richardson.

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The FreeIntv core is licensed under

- [GPLv3](https://github.com/markwkidd/FreeIntv/blob/master/LICENSE)

## Extensions

Content that can be loaded by the FreeIntv core have the following file extensions:

- .int
- .rom
- .bin

## Databases

RetroArch database(s) that are associated with the FreeIntv core:

- [Mattel - Intellivision](https://github.com/libretro/libretro-database/blob/master/rdb/Mattel%20-%20Intellivision.rdb)

## BIOS

FreeIntv requires two Intellivision BIOS files:

|   Filename    |    Description         |              md5sum              |
|:-------------:|:----------------------:|:--------------------------------:|
| exec.bin | Executive ROM | 62e761035cb657903761800f4437b8af |
| grom.bin | Graphics ROM | 0cd5946c6473e42e8e4c2137785e427f |


## Features

RetroArch-level settings or features that the FreeIntv core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | -         |
| Screenshots       | -         |
| Saves             | -         |
| States            | -         |
| Rewind            | -         |
| Netplay           | -         |
| Core Options      | -         |
| RetroAchievements | -         |
| RetroArch Cheats  | -         |
| Native Cheats     | -         |
| Controls          | -         |
| Remapping         | -         |
| Multi-Mouse       | -         |
| Rumble            | -         |
| Sensors           | -         |
| Camera            | -         |
| Location          | -         |
| Subsystem         | -         |
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | -         |
| Disk Control      | -         |
| Username          | -         |
| Language          | -         |
| Crop Overscan     | -         |
| LEDs              | -         |

### Directories

The FreeIntv core's directory name is 'freeintv'

The FreeIntv core saves/loads to/from these directories.

**RetroArch's Home directory**

- retroarch-core-options.cfg (Core-options)

**RetroArch's Config directory**

- freeintv.cfg (Core Overrides)
- 'content-name'.cfg (Game Overrides)
- 'content-name'.opt (Game-options)

**RetroArch's Input Remapping directory**

- freeintv.rmp (Core Remap)
- 'content-name'.rmp (Game Remap)

**RetroArch's System directory**

- . ()

**Loaded content's directory**

- . ()

### Usage

#### Controller overlays
Mattel Intellivision games were often meant to be played with game-specific cards overlaid on the numeric keypad. These overlays convey information which can be very useful in gameplay. Images of a limited selection of Intellivision titles are available at: http://www.intellivisionlives.com/bluesky/games/instructions.shtml

#### Controls
* The libretro 'RetroPad' d-pad will give you 8-way movement. If available, the RetroPad left analog stick will function like the 16-way disc.
* The FreeIntv "mini keypad" allows you to view and press keys on a small keypad that appears in the lower-corner of the display while L or R is being held.
* The "X" button is also mapped to the last selected keypad button, giving quick access. In Astrosmash, for example, you can leave "3" selected to enable instant access to hyperspace.
* The select button lets you switch the left and right controllers. Some games expect the left controller to be player one, others expect the right controller. This isn't a problem if you have two controllers (and don't mind juggling them) but users with only one controller or using a portable setup would be effectively locked out of some games. Pressing select from either controller with swap the left controller for the right and vice-versa.

## Controllers

#### Joypad

| User # Remap descriptors | RetroPad Inputs                              | (Device name) Inputs      |
|--------------------------|----------------------------------------------|---------------------------|
| Action 1                 | ![](images/RetroPad/Retro_B_Round.png)       | -                         |
| Action 2                 | ![](images/RetroPad/Retro_Y_Round.png)       | -                         |
| Action 3                 | ![](images/RetroPad/Retro_Select.png)        | -                         |
| Action 4                 | ![](images/RetroPad/Retro_Start.png)         | -                         |
| Action 5                 | ![](images/RetroPad/Retro_Dpad_Up.png)       | -                         |
| Action 6                 | ![](images/RetroPad/Retro_Dpad_Down.png)     | -                         |
| Action 7                 | ![](images/RetroPad/Retro_Dpad_Left.png)     | -                         |
| Action 8                 | ![](images/RetroPad/Retro_Dpad_Right.png)    | -                         |
| Action 9                 | ![](images/RetroPad/Retro_A_Round.png)       | -                         |
| Action 10                | ![](images/RetroPad/Retro_X_Round.png)       | -                         |
| Action 11                | ![](images/RetroPad/Retro_L1.png)            | -                         |
| Action 12                | ![](images/RetroPad/Retro_R1.png)            | -                         |
| Action 13                | ![](images/RetroPad/Retro_L2.png)            | -                         |
| Action 14                | ![](images/RetroPad/Retro_R2.png)            | -                         |
| Action 15                | ![](images/RetroPad/Retro_L3.png)            | -                         |
| Action 16                | ![](images/RetroPad/Retro_R3.png)            | -                         |
| Action 17                | ![](images/RetroPad/Retro_Left_Stick.png) X  | -                         |
| Action 18                | ![](images/RetroPad/Retro_Left_Stick.png) Y  | -                         |
| Action 19                | ![](images/RetroPad/Retro_Right_Stick.png) X | -                         |
| Action 20                | ![](images/RetroPad/Retro_Right_Stick.png) Y | -                         |

## Compatibility
| Game | Issue |
|------|-------|
| TBD  |       |

## External Links

- [FreeIntv github repository](https://github.com/markwkidd/FreeIntv)
- [Official FreeIntv for RetroPie website]http://neocomputer.org/projects/freeintv/)
- [Libretro FreeIntv Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/freeintv_libretro.info)
