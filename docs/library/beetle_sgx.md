# PC Engine SuperGrafx (Beetle SGX)

## Background

Standalone port of Mednafen PCE Fast to libretro. This one only emulates a SuperGrafx TG-16

### Why use this core?

-

### Author(s):

Mednafen Team

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_sgx.md). Changes are proposed using "Pull Requests."

## See also

[PC Engine/PCE-CD (Beetle PCE FAST)](https://doc.libretro.com/library/beetle_pce_fast/)

[PC-FX (Beetle PC-FX)](https://doc.libretro.com/library/beetle_pcfx/)

## License

GPLv2

## Extensions

*Content that can be loaded by the Beetle SGX core have the following file extensions.*

pce|sgx|cue|ccd|chd

## Database(s)

*RetroArch database(s) that are associated with the Beetle SGX core*

* NEC - PC Engine SuperGrafx

## BIOS

*Required or optional firmware files go in RetroArch's system directory.*

|   Filename    |    Description                        |              md5sum              |
|:-------------:|:-------------------------------------:|:--------------------------------:|
| syscard3.pce  | Super CD-ROM2 System V3.xx - Required | 38179df8f4ac870017db21ebcbf53114 |                                 |
| syscard2.pce  | CD-ROM System V2.xx - Optional        |  -                               |
| syscard1.pce  | CD-ROM System V1.xx - Optional        |  -                               |
| gexpress.pce  | Game Express CD Card- Optional        |  -                               |

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| RetroAchievements | ✔         |
| RetroArch Cheats  | -         |
| Native Cheats     | ✕         |
| Controllers       | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | -         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |

The Beetle SGX core's directory name is 'Mednafen SuperGrafx'

Game data is saved/loaded to and from where save files are stored.

Save states are saved/loaded to and from where state files are stored. 

## Core options

*The Beetle SGX core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.*

- **CD Image Cache (Restart)** (**Off**/On): Loads the complete image in memory at startup.
- **CD Bios (Restart)** (**System Card 3**/Games Express/System Card 1/System Card 2): Select which CD BIOS to use.
- **No Sprite Limit (Restart)** (**Off**/On): Disables the sprite limit.
- **CPU Overclock Multiplier (Restart)** (**1**/2/3/4/5/6/7/8/9/10/20/30/40/50): Awaiting description.
- **Horizontal Overscan (352 Width Mode Only)** (**352**/300/302/304/306/308/310/312/314/316/318/320/322/324/326/328/330/332/334/336/338/340/342/344/346/348/350): Awaiting description.
- **Initial scanline** (**3**/4/5/6/7/8/9/10/11/12/13/14/15/16/17/18/19/20/21/22/23/24/25/26/27/28/29/30/31/32/33/34/35/36/37/38/39/40/0/1/2): First displayed scanline.
- **Last scanline** (**242**|208|209|210|211|212|213|214|215|216|217|218|219|220|221|222|223|224|225|226|227|228|229|230|231|232|233|234|235|236|237|238|239|240|241): Last displayed scanline.
- **(CD) CDDA Volume %** (**100**/110/120/130/140/150/160/170/180/190/200/0/10/20/30/40/50/60/70/80/90): Awaiting description.
- **(CD) ADPCM Volume %** (**100**/110/120/130/140/150/160/170/180/190/200/0/10/20/30/40/50/60/70/80/90): Awaiting description.
- **(CD) CD PSG Volume %** (**100**/110/120/130/140/150/160/170/180/190/200/0/10/20/30/40/50/60/70/80/90): Awaiting description.
- **(CD) CD Speed** (**1**/2/4/8): Set the speed of the emulated CD drive.
- **Turbo Delay** (**3**/4/5/6/7/8/9/10/11/12/13/14/15/30/60/2): Awaiting description.
- **Turbo ON/OFF Toggle** (**Off**/On): Awaiting description.

## Controllers

*The Beetle SGX core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):*

### User 1 - 2 Device Type(s)

* **PCE Joypad** - Joypad - *Awaiting description.*

* Mouse - Mouse - *Awaiting description.*

### User 3 - 16 Device Type(s)

* **RetroPad** - Joypad

### Controllers graph

| Beetle SGX  | RetroPad                                                       |
|-------------|----------------------------------------------------------------|
| II          | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               |
| III         | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)               |
| Select      | ![RetroPad_Select](images/RetroPad/Retro_Select.png)           |
| Run         | ![RetroPad_Start](images/RetroPad/Retro_Start.png)             |
| D-Pad Up    | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            |
| D-Pad Down  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          |
| D-Pad Left  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          |
| D-Pad Right | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         |
| I           | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               |
| IV          | ![RetroPad_X](images/RetroPad/Retro_X_Round.png)               |
| V           | ![RetroPad_L1](images/RetroPad/Retro_L1.png)                   |
| VI          | ![RetroPad_R1](images/RetroPad/Retro_R1.png)                   |
| Mode Switch | ![RetroPad_L2](images/RetroPad/Retro_L2_Temp.png)              |

| RetroMouse                                                      | Mouse |
|-----------------------------------------------------------------|-------|
| ![Retro_Mouse](images/RetroMouse/Retro_Mouse.png)               |  -    |
| ![Retro_Left](images/RetroMouse/Retro_Left.png)                 |  -    |
| ![Retro_Middle](images/RetroMouse/Retro_Middle.png)             |  -    |
| ![Retro_Right](images/RetroMouse/Retro_Right.png)               |  -    |
| ![Retro_Left+Middle](images/RetroMouse/Retro_Left+Middle.png)   |  -    |
| ![Retro_Right+Middle](images/RetroMouse/Retro_Right+Middle.png) |  -    |

## Compatibility

Unknown

## External Links

* [Libretro Repository](https://github.com/libretro/beetle-supergrafx-libretro)
* [Report Core Issues Here](https://github.com/libretro/libretro-meta)
* [Official Website](http://mednafen.sourceforge.net/)
* [Official Upstream Downloads](https://mednafen.github.io/releases/)