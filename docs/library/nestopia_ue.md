# NES / Famicom (Nestopia UE)

## Background

Nestopia is a portable and cycle-accurate NES/Famicom emulator written in C++. Nestopia UE (Undead Edition) is a fork of the original source code, with enhancements from members of the emulation community. This includes support for new platforms, and bug fixes in the emulator core. 

### Why use this core?

-

### Author(s)

Martin Freij|R. Belmont|R. Danbrook

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/nestopia_ue.md). Changes are proposed using "Pull Requests."

## See also

[NES / Famicom (bnes)](https://doc.libretro.com/library/bnes/)

[NES / Famicom (Emux)](https://doc.libretro.com/library/emux_nes/)

[NES / Famicom (FCEUmm)](https://doc.libretro.com/library/fceumm/)

[NES / Famicom (QuickNES)](https://doc.libretro.com/library/quicknes/)

## License

GPLv2

## Extensions

*Content that can be loaded by the Nestopia UE core have the following file extensions.*

nes|fds|unf|unif

## Database(s)

*RetroArch database(s) that are associated with the Nestopia UE core*

* Nintendo - Nintendo Entertainment System

* Nintendo - Family Computer Disk System

## BIOS

*Required or optional firmware files go in RetroArch's system directory.*

|   Filename    |    Description                                                                |              md5sum              |
|:-------------:|:-----------------------------------------------------------------------------:|:--------------------------------:|
| disksys.rom   | Family Computer Disk System BIOS - Required for Famicom Disk System emulation | ca30b50f880eb660a320674ed365ef7a |

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
| Remapping         | ✔         |
| Multi-Mouse       | -         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |

The Nestopia UE core's directory name is 'Nestopia'

Game data is saved/loaded to and from where save files are stored.

Save states are saved/loaded to and from where state files are stored. 

## Core options

*The Nestopia UE core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.*

- **Blargg NTSC filter** (**Off**/composite/svideo/rgb/monochrome): Enable Blargg NTSC filters.
- **Palette** (**cxa2025as**/consumer/canonical/alternative/rgb/pal/composite-direct-fbx/pvm-style-d93-fbx/ntsc-hardware-fbx/nes-classic-fbx-fs/raw/custom): Choose which color palette is going to be used.
- **Remove 8-sprites-per-scanline hardware limit** (**Off**/On): Self-explanatory.
- **CPU Speed (Overclock)** (**1x**/2x): Awaiting description.
- **Automatically insert first FDS disk on reset** (Off/**On**): Self-explanatory
- **Mask Overscan (Vertical)** (Off/**On**): Awaiting description.
- **Mask Overscan (Horizontal)** (**Off**/On): Awaiting description.
- **Preferred aspect ratio** (**auto**/ntsc/pal/4:3): Awaiting description.
- **Game Genie Sound Distortion** (**Off**/On): Awaiting description.
- **Favored System** (**auto**/ntsc/pal/famicom/dendy): Awaiting description.
- **RAM Power-on State** (**0x00**/0xFF/random): Awaiting description.
- **Turbo Pulse Speed** (**2**/3/4/5/6/7/8/9): Awaiting description.

## Controllers

*The Nestopia UE core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):*

### User 1 - 16 Device Type(s)

* **RetroPad** - Joypad

* RetroPad w/Analog - Joypad - **There is no reason to switch to this.**

### Controllers graph

| Nestopia UE | RetroPad                                                       |
|-------------|----------------------------------------------------------------|
| B           | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               |
| Turbo B     | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)               |
| Select      | ![RetroPad_Select](images/RetroPad/Retro_Select.png)           |
| Start       | ![RetroPad_Start](images/RetroPad/Retro_Start.png)             |
| D-Pad Up    | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            |
| D-Pad Down  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          |
| D-Pad Left  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          |
| D-Pad Right | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         |
| A           | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               |
| Turbo A     | ![RetroPad_X](images/RetroPad/Retro_X_Round.png)               |
| (FDS) Disk Side Change   | ![RetroPad_L1](images/RetroPad/Retro_L1.png)      |
| (FDS) Eject Disk   | ![RetroPad_R1](images/RetroPad/Retro_R1.png)            |
| (VSSystem) Coin 1)   | ![RetroPad_L2](images/RetroPad/Retro_L2_Temp.png)     |
| (VSSystem Coin 2)   | ![RetroPad_R2](images/RetroPad/Retro_R2.png)           |
| (Famicom) Microphone   | ![RetroPad_L3](images/RetroPad/Retro_L3.png)        |

## Compatibility

| Game                   | Issue                                                            |
|------------------------|----------------------------------------------------------------- |
| Skull & Crossbones     | Graphical glitches and screen shaking when in 2-player mode. (1) |

??? note "(1)"
	![skull&crossbones_graphicalglitches](images/Cores/nestopia_ue/skull&crossbones_graphicalglitches.png)

## External Links

* [Libretro Github Repository](https://github.com/libretro/nestopia)
* [Report Core Issues Here](https://github.com/libretro/libretro-meta)
* [Official Website](http://0ldsk00l.ca/nestopia/)
* [Official Github Repository](https://github.com/rdanbrook/nestopia)