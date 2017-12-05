# NES / Famicom (FCEUmm)

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/fceumm.md). Changes are proposed using "Pull Requests."

## Background

FCEU "mappers modified" is an unofficial build of FCEU Ultra by CaH4e3, which supports a lot of new mappers including some obscure mappers such as one for unlicensed NES ROM's.

### Why use this core?

Awaiting description.

### How to get and install the FCEUmm core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'NES / Famicom (FCEUmm)'.

After this has finished downloading, the core should now be ready for use!

### Authors

- FCEU Team
- CaH4e3

## See also

- [NES / Famicom (bnes)](https://docs.libretro.com/library/bnes/) - Shared platforms
- [NES / Famicom (Emux)](https://docs.libretro.com/library/emux_nes/) - Shared platforms
- [NES / Famicom (Nestopia UE)](https://docs.libretro.com/library/nestopia_ue/) - Shared platforms
- [NES / Famicom (QuickNES)](https://docs.libretro.com/library/quicknes/) - Shared platforms

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

- [GPLv2](https://github.com/libretro/libretro-fceumm/blob/master/Copying)

## Extensions

Content that can be loaded by the FCEUmm core have the following file extensions:

- .fds
- .nes
- .unif
- .unf

## Databases

RetroArch database(s) that are associated with the FCEUmm core:

* [Nintendo - Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Nintendo%20Entertainment%20System.rdb)
* [Nintendo - Family Computer Disk System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Family%20Computer%20Disk%20System.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

|   Filename    |    Description                                                                                                               | md5sum                           |
|:-------------:|:----------------------------------------------------------------------------------------------------------------------------:|:--------------------------------:|
| disksys.rom   | Family Computer Disk System BIOS - Required for Famicom Disk System emulation                                                | ca30b50f880eb660a320674ed365ef7a |
| nes.pal       | Custom NES Palette [(Color Palette core option)](https://docs.libretro.com/library/fceumm/#core-options) - Optional          |                                  |

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| RetroAchievements | ✔         |
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
| Softpatching      | ✔         |
| Disk Control      | ✕         |

### Saves/States

The FCEUmm core's directory name is 'FCEUmm'

Game data is saved/loaded to and from where save files are stored.

- .srm (Battery save)

Save states are saved/loaded to and from where state files are stored.

- .state (State)

### Core provided aspect ratio

The core provided aspect ratio can be configured with the ['Preferred aspect ratio' core option](https://docs.libretro.com/library/fceumm/#core-options).

### Crop overscan

Cropping overscan can be configured with the ['Crop Overscan (Horizontal)' and 'Crop Overscan (Vertical)' core options](https://docs.libretro.com/library/fceumm/#core-options).

### Custom color palettes

To use custom color palettes in the FCEUmm core, the Color Palette core option must be set to custom and the custom color palette file you want to use must be in RetroArch's system directory. Make sure the custom palette file is named 'nes.pal'

Custom color palettes for the NES can be generated with either of these tools.

- [Bisqwit's NTSC NES palette generator](http://bisqwit.iki.fi/utils/nespalette.php)
- [Drag's NTSC NES palette generator](http://drag.wootest.net/misc/palgen.html)

## Core options

The FCEUmm core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.

- **Region Override** (**Auto**/NTSC/PAL/Dendy): Choose which region the system is from.
- **Preferred aspect ratio** (**8:7 PAR**/4:3): Choose the preferred aspect ratio. RetroArch's aspect ratio must be set to Core provided in the Video seetings.

??? note "Preferred aspect ratio - 8:7 PAR"
	![8by7_PAR](images\Cores\fceumm\8by7_PAR.png)
	
??? note "Preferred aspect ratio - 4:3"
	![4by3](images\Cores\fceumm\4by3.png)

- **Color Palette** (**default**/asqrealc/nintendo-vc/rgb/yuv-v3/unsaturated-final/sony-cxa2025as-us/pal/bmf-final2/bmf-final3/smooth-fbx/composite-direct-fbx/pvm-style-d93-fbx/ntsc-hardware-fbx/nes-classic-fbx-fs/nescap/wavebeam/raw/custom): Choose which color palette is going to be used. The raw palette can used in combination with the nes-decoder shader to give colors based off on Bisqwit's NES palette generator and applies either an FCC color conversion matrix or specific Sony US matrix.

!!! attention ""
	**These 'Color Palette core option screenshots have been taken with the 'Use NTSC Palette' core option set to Off.**

??? note "Color Palette - default"
	![color_palette_default](images\Cores\fceumm\color_palette_default.png)

??? note "Color Palette - asqrealc"
	![color_palette_asqrealc](images\Cores\fceumm\color_palette_asqrealc.png)

??? note "Color Palette - nintendo-vc"
	![color_palette_nintendo_vc](images\Cores\fceumm\color_palette_nintendo_vc.png)

??? note "Color Palette - rgb"
	![color_palette_rgb](images\Cores\fceumm\color_palette_rgb.png)

??? note "Color Palette - yuv-v3"
	![color_palette_yuv_v3](images\Cores\fceumm\color_palette_yuv_v3.png)

??? note "Color Palette - unsaturated-final"
	![color_palette_unsaturated_final](images\Cores\fceumm\color_palette_unsaturated_final.png)

??? note "Color Palette - sony-cxa2025as-us"
	![color_palette_sony_cxa2025as_us](images\Cores\fceumm\color_palette_sony_cxa2025as_us.png)

??? note "Color Palette - pal"
	![color_palette_pal](images\Cores\fceumm\color_palette_pal.png)

??? note "Color Palette - bmf-final2"
	![color_palette_bmf_final2](images\Cores\fceumm\color_palette_bmf_final2.png)

??? note "Color Palette - bmf-final3"
	![color_palette_bmf_final3](images\Cores\fceumm\color_palette_bmf_final3.png)

??? note "Color Palette - smooth-fbx"
	![color_palette_smooth_fbx](images\Cores\fceumm\color_palette_smooth_fbx.png)
	
??? note "Color Palette - composite-direct-fbx"
	![color_palette_composite_direct-fbx](images\Cores\fceumm\color_palette_composite_direct_fbx.png)

??? note "Color Palette - pvm-style-d93-fbx"
	![color_palette_pvm_style_d93_fbx](images\Cores\fceumm\color_palette_pvm_style_d93_fbx.png)

??? note "Color Palette - ntsc-hardware-fbx"
	![color_palette_ntsc_hardware_fbx](images\Cores\fceumm\color_palette_ntsc_hardware_fbx.png)

??? note "Color Palette - nes-classic-fbx-fs"
	![color_palette_nes_classic_fbx_fs](images\Cores\fceumm\color_palette_nes_classic_fbx_fs.png)

??? note "Color Palette - nescap"
	![color_palette_nescap](images\Cores\fceumm\color_palette_nescap.png)

??? note "Color Palette - wavebeam"
	![color_palette_wavebeam](images\Cores\fceumm\color_palette_wavebeam.png)

??? note "Color Palette - raw"
	![color_palette_raw](images\Cores\fceumm\color_palette_raw.png)	

- **Use NTSC Palette** (**Off**/On): Self-explanatory.

!!! attention ""
	**These 'Use NTSC Palette' core option screenshots have been taken with the 'Color Palette' core option set to default.**

??? note "Use NTSC Palette - Off"
	![use_ntsc_palette_off](images\Cores\fceumm\use_ntsc_palette_off.png)
	
??? note "Use NTSC Palette - On"
	![use_ntsc_palette_on](images\Cores\fceumm\use_ntsc_palette_on.png)	

- **Crop Overscan (Horizontal)** (**Off**/On): Crop out (horizontally) the potentially random glitchy video output that would have been hidden by the bezel around the edge of a standard-definition television screen.

??? note "Crop Overscan (Horiontal) - Off"
	![crop_overscan_horizontal_off](images\Cores\fceumm\crop_overscan_horizontal_off.png)
	
??? note "Crop Overscan (Horizontal) - On"
	![crop_overscan_horizontal_on](images\Cores\fceumm\crop_overscan_horizontal_on.png)	

- **Crop Overscan (Vertical)** (Off/**On**): Crop out (vertically) the potentially random glitchy video output that would have been hidden by the bezel around the edge of a standard-definition television screen.

??? note "Crop Overscan (Vertical) - On"
	![crop_overscan_vertical_on](images\Cores\fceumm\crop_overscan_vertical_on.png)
	
??? note "Crop Overscan (Vertical) - Off"
	![crop_overscan_vertical_off](images\Cores\fceumm\crop_overscan_vertical_off.png)	

- **No Sprite Limit** (**Off**/On):  Removes 8-sprites-per-scanline hardware limit.
- **Sound Volume** (**150**/160/170/180/190/200/210/220/230/240/250/0/10/20/30/40/50/60/70/80/90/100/110/120/130/140): Self-explanatory.
- **Sound Quality** (**Low**/High/Very High): Enables high/higher sound quality for games using expansion audio (MMC5, VRC6, VRC7, Namco, Sunsoft). Use Low for slower devices.
- **Swap Duty Cycles** (**Off**/On): Replicates the sound of some famiclones that have duty cycles swapped for square channels. A quick sound comparison is in Contra's sound effect when shooting with normal bullets.
- **Turbo Enable** (**None**/Player 1/Player 2/Both): Enable the use of the [Turbo B and Turbo A buttons](https://docs.libretro.com/library/fceumm/index.html#controller-tables).
- **Turbo Delay (in frames)** (**3**/5/10/15/30/60/1/2): The number of frames between consecutive buttton presses when the Turbo B or Turbo A buttons are held down.
- **Zapper Mode** (**pointer**/mouse): Pointer allows the Zapper Device Type to be used for touch-devices, but still can be used with regular mouse. Pointer and Mouse mode movement behaves differently with different input driver so user can choose which movement feels natural to them.
- **Show Crosshair** (Off/**On**): Show the crosshair for the Zapper device type.

??? note "Show Crosshair - On"
	![show_crosshair_on](images\Cores\fceumm\show_crosshair_on.png)
	
??? note "Show Crosshair - Off"
	![show_crosshair_off](images\Cores\fceumm\show_crosshair_off.png)	

- **Overclocking** (**Off**/2x-Postrender/2x-VBlank): Overclocks the NES using PPU method to minimize ingame slowdowns of some games. Contra Force needs VBlank mode (stage 3 slowdowns). Choose which ever minimizes slowdowns without image distortion.

## Controllers

### Device types

The FCEUmm core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- **Auto** - Joypad - Based off the loaded game's crc, the core will automatically select a regular controller (NES or Famicom) for User 1.

- [Gamepad](http://nintendo.wikia.com/wiki/Nintendo_Entertainment_System_controller) - Joypad - Manually selects a regular controller (NES or Famicom) for User 1.

- [Zapper](http://nintendo.wikia.com/wiki/NES_Zapper) - Mouse - Manually selects a Zapper light gun (NES or Famicom) for User 1.

#### User 2 device types

- **Auto** - Joypad - Based off the loaded game's crc, the core will automatically select a regular controller (NES or Famicom) or a Zapper light gun (NES or Famicom) or a Arkanoid Paddle (NES only) for User 2.

- [Gamepad](http://nintendo.wikia.com/wiki/Nintendo_Entertainment_System_controller) - Joypad - Manually selects a regular controller (NES or Famicom) for User 2.

- [Arkanoid](https://en.wikipedia.org/wiki/Arkanoid_Controller) - Mouse - Manually selects a Arkanoid Paddle (NES only) for User 2.

- [Zapper](http://nintendo.wikia.com/wiki/NES_Zapper) - Mouse - Manually selects a Zapper light gun (NES or Famicom) for User 2.

### Other Famicom controllers

The FCEUmm core will also auto select the following controllers for the Famicom based off the loaded game's crc.

- Arkanoid Paddle (Famicom) - Mouse

- Bandai Hyper Shot Gun (Famicom) - Mouse

- Oeka Kids Tablet (Famicom) - Mouse

!!! warning ""
	Please note that these Famicom controllers are completely separate from the device types in the controls menu and cannot be manually selected.

### Controller tables

#### Joypad and analog device type table

!!! warning ""
	In order to use the Turbo A and Turbo B buttons, the 'Turbo Enable' core option must be set to On.

| FCEUmm input descriptors      | User 1 RetroPad                              | Gamepad                 |
|-------------------------------|----------------------------------------------|-------------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                       |
| Turbo B                       | ![](images/RetroPad/Retro_Y_Round.png)       | Turbo B                 |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select                  |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start                   |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up                |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down              |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left              |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right             |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | A                       |
| Turbo A                       | ![](images/RetroPad/Retro_X_Round.png)       | Turbo A                 |
| (FDS) Disk Side Change        | ![](images/RetroPad/Retro_L1.png)            | (FDS) Disk Side Change  |
| (FDS) Insert/Eject Disk       | ![](images/RetroPad/Retro_R1.png)            | (FDS) Insert/Eject Disk |
| (VSSystem) Insert Coin        | ![](images/RetroPad/Retro_R2.png)            | (VSSystem) Insert Coin  |

| FCEUmm input descriptors      | Users 2 - 4 RetroPad                         | Gamepad            |
|-------------------------------|----------------------------------------------|--------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                  |
| Turbo B                       | ![](images/RetroPad/Retro_Y_Round.png)       | Turbo B            |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select             |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start              |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up           |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down         |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left         |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right        |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | A                  |
| Turbo A                       | ![](images/RetroPad/Retro_X_Round.png)       | Turbo A            |

#### Mouse device type table

| FCEUmm input descriptors      | RetroMouse                               | Zapper             | Arkanoid   | Oeka Kids Tablet   | Bandai Hyper Shot Gun   |
|-------------------------------|------------------------------------------|--------------------|------------|--------------------|-------------------------|
| **                            | ![](images/RetroMouse/Retro_Mouse.png) X | Zapper X           | Arkanoid X | Oeka Kids Tablet X | Bandai Hyper Shot Gun X |  
| **                            | ![](images/RetroMouse/Retro_Mouse.png) Y | Zapper Y           | Arkanoid Y | Oeka Kids Tablet Y | Bandai Hyper Shot Gun Y |
| **                            | ![](images/RetroMouse/Retro_Left.png)    | Trigger            | Fire       | Touch              | Shoot                   |

!!! warning ""
	When the 'Zapper' device type is changed to a Pointer device type with the ['Zapper Mode' core option](https://buildbot.libretro.com/.docs/library/fceumm/#core-options), the inputs will be the exact same.
	
### Multitap support

The FCEUmm core supports up to 4 players in multitap games for the NES and Famicom, games with multitap usage are detected by their crc.
	
## Compatibility

| Game                         | Issue                                                        |
|------------------------------|--------------------------------------------------------------|
| Skull & Crossbones           | Graphical glitches and screen shaking when in 2-player mode. | 

## External Links

- [Libretro FCEUmm Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/fceumm_libretro.info)
- [Libretro FCEUmm Github Repository](https://github.com/libretro/libretro-fceumm)
- [Report Libretro FCEUmm Core Issues Here](https://github.com/libretro/libretro-fceumm/issues)
- [Official FCEUmm Website](http://cah4e3.shedevr.org.ru/fceultra.php)
- [Official FCEUmm Sourceforge Repository](https://sourceforge.net/projects/fceumm/)