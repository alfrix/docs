# 3DO (4DO)

## Background

4DO is an open-source, low-level emulator for the 3DO Game Console based on the FreeDO source code.

### Author(s):

JohnnyDude|FreeDO team

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/4DO.md). Changes are proposed using "Pull Requests."

## License

Non-commercial

## Extensions

*Content that can be loaded by the 4DO core have the following file extensions.*

iso|cue

## Database(s)

*RetroArch databases that are associated with the 4DO core*

* The 3DO Company - 3DO

## BIOS

*Required or optional firmware files go in RetroArch's system directory.*

|   Filename    |    Description                  |              md5sum              |
|:-------------:|:-------------------------------:|:--------------------------------:|
| panafz10.bin  | Panasonic FZ-10 BIOS - Required | 51f2f43ae2f3508a14d9f56597e2d3ce |

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| RetroAchievements | ✕         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controllers       | ✔         |
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |

The 4DO core's directory name is '4DO'

Game data is saved/loaded to and from where save files are stored.

Save states are saved/loaded to and from where state files are stored. 

## Core options

*The 4DO core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.*

- **High Resolution (restart)** (**Off**/On): Doubles internal resolution.

??? note "High Resolution - Off"
	![high_resolution_off](images\Cores\4do\high_resolution_off.png)
	
??? note "High Resolution - On"
	![high_resolution_on](images\Cores\4do\high_resolution_on.png)
	
## Controllers

*The 4DO core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):*

### User 1 - 16 Device Type(s)

* **RetroPad** - Joypad with analog

* RetroPad w/Analog - **No reason to switch to this**

### Controllers graph

| 4DO            | RetroPad                                                       |
|----------------|----------------------------------------------------------------|
| B              | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               |
| A              | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)               |
| X (Stop)       | ![RetroPad_Select](images/RetroPad/Retro_Select.png)           |
| P (Play/Pause) | ![RetroPad_Start](images/RetroPad/Retro_Start.png)             |
| D-Pad Up       | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            |
| D-Pad Down     | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          |
| D-Pad Left     | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          |
| D-Pad Right    | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         |
| C              | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               |
| L              | ![RetroPad_L1](images/RetroPad/Retro_L1.png)                   |
| R              | ![RetroPad_R1](images/RetroPad/Retro_R1.png)                   |

## Compatibility

[4DO Core Compatibility List](http://wiki.fourdo.com/Compatibility_List)

## External Links

* [Libretro Repository](https://github.com/libretro/4do-libretro)
* [Report Core Issues Here](https://github.com/libretro/libretro-meta)
* [Official Website](http://www.fourdo.com/)
* [Official Repository](https://sourceforge.net/projects/fourdo/)
