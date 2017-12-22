# NES / Famicom (FCEUmm)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/fceumm.md). Changes are proposed using "Pull Requests."

There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)

You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).

## Background

FCEU "mappers modified" is an unofficial build of FCEU Ultra by CaH4e3, which supports a lot of new mappers including some obscure mappers such as one for unlicensed NES ROM's.

### Why use this core?

Awaiting description.

### How to get and install the FCEUmm core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'NES / Famicom (FCEUmm)'.

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'NES / Famicom (FCEUmm)'.

The content should now start running!

### Authors

- FCEU Team
- CaH4e3

## See also

### NES/Famicom

- [NES / Famicom (bnes)](https://docs.libretro.com/library/bnes/)
- [NES / Famicom (Emux)](https://docs.libretro.com/library/emux_nes/)
- [NES / Famicom (Nestopia UE)](https://docs.libretro.com/library/nestopia_ue/)
- [NES / Famicom (QuickNES)](https://docs.libretro.com/library/quicknes/)

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

RetroArch-level settings or features that the FCEUmm core respects.

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
| Softpatching      | ✔         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The FCEUmm core's directory name is 'FCEUmm'

The FCEUmm core saves/loads from/to these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The FCEUmm core's internal FPS is (FPS)
- The FCEumm core's internal sample rate is (Rate)
- The FCEUmm core's core provided aspect ratio is dependent on the ['Preferred aspect ratio' core option](https://docs.libretro.com/library/fceumm/#core-options).

### Custom color palettes

To use custom color palettes in the FCEUmm core, the ['Color Palette' core option](https://docs.libretro.com/library/fceumm/#core-options) must be set to custom and the custom color palette file you want to use must be in RetroArch's system directory. 

Make sure the custom palette file is named 'nes.pal'

Custom color palettes for the NES can be generated with either of these tools.

- [Bisqwit's NTSC NES palette generator](http://bisqwit.iki.fi/utils/nespalette.php)
- [Drag's NTSC NES palette generator](http://drag.wootest.net/misc/palgen.html)

## Core options

The FCEUmm core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Region Override** (**Auto**/NTSC/PAL/Dendy)

<center> Choose which region the system is from. </center>

- **Preferred aspect ratio** (**8:7 PAR**/4:3)

<center> Choose the preferred aspect ratio. RetroArch's aspect ratio must be set to Core provided in the Video seetings. </center>

??? note "Preferred aspect ratio - 8:7 PAR"
	![](images\Cores\fceumm\8by7_PAR.png)
	
??? note "Preferred aspect ratio - 4:3"
	![](images\Cores\fceumm\4by3.png)

- **Color Palette** (**default**/asqrealc/nintendo-vc/rgb/yuv-v3/unsaturated-final/sony-cxa2025as-us/pal/bmf-final2/bmf-final3/smooth-fbx/composite-direct-fbx/pvm-style-d93-fbx/ntsc-hardware-fbx/nes-classic-fbx-fs/nescap/wavebeam/raw/custom)

<center> Choose which color palette is going to be used. The raw palette can used in combination with the nes-decoder shader to give colors based off on Bisqwit's NES palette generator and applies either an FCC color conversion matrix or specific Sony US matrix. </center>

!!! attention
	These 'Color Palette core option screenshots have been taken with the 'Use NTSC Palette' core option set to Off.

??? note "Color Palette - default"
	![](images\Cores\fceumm\default.png)

??? note "Color Palette - asqrealc"
	![](images\Cores\fceumm\asqrealc.png)

??? note "Color Palette - nintendo-vc"
	![](images\Cores\fceumm\nintendo_vc.png)

??? note "Color Palette - rgb"
	![](images\Cores\fceumm\rgb.png)

??? note "Color Palette - yuv-v3"
	![](images\Cores\fceumm\yuv_v3.png)

??? note "Color Palette - unsaturated-final"
	![](images\Cores\fceumm\unsaturated_final.png)

??? note "Color Palette - sony-cxa2025as-us"
	![](images\Cores\fceumm\sony_cxa2025as_us.png)

??? note "Color Palette - pal"
	![](images\Cores\fceumm\pal.png)

??? note "Color Palette - bmf-final2"
	![](images\Cores\fceumm\bmf_final2.png)

??? note "Color Palette - bmf-final3"
	![](images\Cores\fceumm\bmf_final3.png)

??? note "Color Palette - smooth-fbx"
	![](images\Cores\fceumm\smooth_fbx.png)
	
??? note "Color Palette - composite-direct-fbx"
	![](images\Cores\fceumm\direct_fbx.png)

??? note "Color Palette - pvm-style-d93-fbx"
	![](images\Cores\fceumm\pvm_style_d93_fbx.png)

??? note "Color Palette - ntsc-hardware-fbx"
	![](images\Cores\fceumm\ntsc_hardware_fbx.png)

??? note "Color Palette - nes-classic-fbx-fs"
	![](images\Cores\fceumm\nes_classic_fbx_fs.png)

??? note "Color Palette - nescap"
	![](images\Cores\fceumm\nescap.png)

??? note "Color Palette - wavebeam"
	![](images\Cores\fceumm\wavebeam.png)

??? note "Color Palette - raw"
	![](images\Cores\fceumm\raw.png)	

- **Use NTSC Palette** (**Off**/On)

<center> Self-explanatory. </center>

!!! attention
	These 'Use NTSC Palette' core option screenshots have been taken with the 'Color Palette' core option set to default.

??? note "Use NTSC Palette - Off"
	![](images\Cores\fceumm\ntsc_off.png)
	
??? note "Use NTSC Palette - On"
	![](images\Cores\fceumm\ntsc_on.png)	

- **Crop Overscan (Horizontal)** (**Off**/On)

<center> Crop out (horizontally) the potentially random glitchy video output that would have been hidden by the bezel around the edge of a standard-definition television screen. </center>

??? note "Crop Overscan (Horiontal) - Off"
	![](images\Cores\fceumm\horiz_off.png)
	
??? note "Crop Overscan (Horizontal) - On"
	![](images\Cores\fceumm\horiz_on.png)	

- **Crop Overscan (Vertical)** (Off/**On**)

<center> Crop out (vertically) the potentially random glitchy video output that would have been hidden by the bezel around the edge of a standard-definition television screen. </center>

??? note "Crop Overscan (Vertical) - On"
	![](images\Cores\fceumm\vert_on.png)
	
??? note "Crop Overscan (Vertical) - Off"
	![](images\Cores\fceumm\vert_off.png)	

- **No Sprite Limit** (**Off**/On)

<center> Removes 8-sprites-per-scanline hardware limit. </center>

- **Sound Volume** (**150**/160/170/180/190/200/210/220/230/240/250/0/10/20/30/40/50/60/70/80/90/100/110/120/130/140)

<center> Self-explanatory. </center>

- **Sound Quality** (**Low**/High/Very High)

<center> Enables high/higher sound quality for games using expansion audio (MMC5, VRC6, VRC7, Namco, Sunsoft). Use Low for slower devices. </center>

- **Swap Duty Cycles** (**Off**/On) 

<center> Replicates the sound of some famiclones that have duty cycles swapped for square channels. A quick sound comparison is in Contra's sound effect when shooting with normal bullets. </center>

- **Turbo Enable** (**None**/Player 1/Player 2/Both)

<center> Enable the use of the [Turbo B and Turbo A buttons](https://docs.libretro.com/library/fceumm/index.html#controllers). </center>

- **Turbo Delay (in frames)** (**3**/5/10/15/30/60/1/2)

<center> The number of frames between consecutive buttton presses when the Turbo B or Turbo A buttons are held down. </center>

- **Zapper Mode** (**pointer**/mouse)

<center> Pointer allows the Zapper Device Type to be used for touch-devices, but still can be used with regular mouse. Pointer and Mouse mode movement behaves differently with different input driver so user can choose which movement feels natural to them. </center>

- **Show Crosshair** (Off/**On**) 

<center> Show the crosshair for the Zapper device type. </center>

??? note "Show Crosshair - On"
	![](images\Cores\fceumm\cross_on.png)
	
??? note "Show Crosshair - Off"
	![](images\Cores\fceumm\cross_off.png)	

- **Overclocking** (**Off**/2x-Postrender/2x-VBlank)

<center> Overclocks the NES using PPU method to minimize ingame slowdowns of some games. Contra Force needs VBlank mode (stage 3 slowdowns). Choose which ever minimizes slowdowns without image distortion. </center>

## Controllers

### Device types

The FCEUmm core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Input disabled.
- **Auto** - Joypad - Based off the loaded game's crc, the core will automatically select a regular controller (NES or Famicom) for User 1.
- [Gamepad](http://nintendo.wikia.com/wiki/Nintendo_Entertainment_System_controller) - Joypad - Manually selects a regular controller (NES or Famicom) for User 1.
- [Zapper](http://nintendo.wikia.com/wiki/NES_Zapper) - Mouse - Manually selects a Zapper light gun (NES or Famicom) for User 1.

#### User 2 device types

- None - Input disabled.
- **Auto** - Joypad - Based off the loaded game's crc, the core will automatically select a regular controller (NES or Famicom) or a Zapper light gun (NES or Famicom) or a Arkanoid Paddle (NES only) for User 2.
- [Gamepad](http://nintendo.wikia.com/wiki/Nintendo_Entertainment_System_controller) - Joypad - Manually selects a regular controller (NES or Famicom) for User 2.
- [Arkanoid](https://en.wikipedia.org/wiki/Arkanoid_Controller) - Mouse - Manually selects a Arkanoid Paddle (NES only) for User 2.
- [Zapper](http://nintendo.wikia.com/wiki/NES_Zapper) - Mouse - Manually selects a Zapper light gun (NES or Famicom) for User 2.

### Other controllers

The FCEUmm core will also auto select the following controllers for the **Famicom** based off the loaded game's crc.

- [Arkanoid Paddle (Famicom)]((https://en.wikipedia.org/wiki/Arkanoid_Controller)) - Mouse
- Bandai Hyper Shot Gun (Famicom) - Mouse
- Oeka Kids Tablet (Famicom) - Mouse

!!! warning
	Please note that these Famicom controllers are completely separate from the device types in the controls menu and cannot be manually selected.

### Multitap support

The FCEUmm core supports up to 4 players in multitap games for the NES and Famicom, games with multitap usage are detected by their crc.
	
### Controller tables

#### Joypad and analog device type table

!!! warning 
	In order to use the Turbo A and Turbo B buttons, the 'Turbo Enable' core option must be set to On.

| User 1 input descriptors      | RetroPad Inputs                              | Gamepad                 |
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

| Users 2 - 4 Input descriptors | RetroPad Inputs                              | Gamepad            |
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
| N/A                           | ![](images/RetroMouse/Retro_Mouse.png)   | Zapper             | Arkanoid   | Oeka Kids Tablet   | Bandai Hyper Shot Gun   |
| N/A                           | ![](images/RetroMouse/Retro_Left.png)    | Trigger            | Fire       | Touch              | Shoot                   |

!!! warning ""
	When the 'Zapper' device type is changed to a Pointer device type with the ['Zapper Mode' core option](https://docs.libretro.com/library/fceumm/index.html#controller-tables), the inputs will be the exact same.

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