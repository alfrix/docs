# Nintendo - NES / Famicom (bnes)

## Background

A port of bNES v083 to libretro.

### Author/License

The bnes core has been authored by

- byuu
- Ryphecha

The bnes core is licensed under

- [GPLv3](https://github.com/libretro/bnes-libretro/blob/master/license)

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

## Extensions

Content that can be loaded by the bnes core have the following file extensions:

- .nes

## Databases

RetroArch database(s) that are associated with the bnes core:

- [Nintendo - Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Nintendo%20Entertainment%20System.rdb)

## Features

Frontend-level settings or features that the bnes core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
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
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | ✔         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |
| LEDs              | ✕         |

### Directories

The bnes core's directory name is 'bnes'

The bnes core saves/loads to/from these directories.

**Frontend's Save directory**

- 'content-name'.srm (Cartridge battery save)

**Frontend's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The bnes core's core provided FPS is 60
- The bnes core's core provided sample rate is 32000 Hz
- The bnes core's core provided aspect ratio is 16/15

## Controllers

The bnes core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 - 2 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There is no reason to switch to this.

### Controller tables

![](images/Controllers/nes.png)

#### Joypad

| User 1 - 2 Remap descriptors | RetroPad Inputs                           |
|------------------------------|-------------------------------------------|
| B                            | ![](images/RetroPad/Retro_B_Round.png)    |
| Select                       | ![](images/RetroPad/Retro_Select.png)     |
| Start                        | ![](images/RetroPad/Retro_Start.png)      |
| D-Pad Up                     | ![](images/RetroPad/Retro_Dpad_Up.png)    |
| D-Pad Down                   | ![](images/RetroPad/Retro_Dpad_Down.png)  |
| D-Pad Left                   | ![](images/RetroPad/Retro_Dpad_Left.png)  |
| D-Pad Right                  | ![](images/RetroPad/Retro_Dpad_Right.png) |
| A                            | ![](images/RetroPad/Retro_A_Round.png)    |

## Compatibility

| Game                         | Issue                                          |
|------------------------------|------------------------------------------------|
| Crisis Force                 | Graphical glitches. (1)                        |
| Huge Insect                  | No enemies spawn.                              |
| Lagrange Point               | No music.                                      |
| Ms. Pac-Man (Tengen version) | Graphical glitches on the sides of the screen. |
| Skull & Crossbones           | Crashes on start.                              |

??? note "(1)"
    ![](images/Cores/bnes/crisisforce.png)

## External Links

- [Official higan Website](https://byuu.org/)
- [Official higan Downloads](https://byuu.org/emulation/higan/)
- [Libretro bnes Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/bnes_libretro.info)
- [Libretro bnes Github Repository](https://github.com/libretro/bnes-libretro)
- [Report Libretro bnes Core Issues Here](https://github.com/libretro/bnes-libretro/issues)

### See also

#### Nintendo - Nintendo Entertainment System

- [Nintendo - NES / Famicom (Emux NES)](https://docs.libretro.com/library/emux_nes/)
- [Nintendo - NES / Famicom (FCEUmm)](https://docs.libretro.com/library/fceumm/)
- [Nintendo - NES / Famicom (Mesen)](https://docs.libretro.com/library/mesen/)
- [Nintendo - NES / Famicom (Nestopia UE)](https://docs.libretro.com/library/nestopia_ue/)
- [Nintendo - NES / Famicom (QuickNES)](https://docs.libretro.com/library/quicknes/)