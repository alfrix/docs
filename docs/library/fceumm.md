# NES / Famicom (FCEUmm)

## Background

FCEU "mappers modified" is an unofficial build of FCEU Ultra by CaH4e3, which supports a lot of new mappers including some obscure mappers such as one for unlicensed NES ROM's.

### Why use this core?

-

### Author(s)

FCEU Team|CaH4e3

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/fceumm.md). Changes are proposed using "Pull Requests."

## See also

[NES / Famicom (bnes)](https://doc.libretro.com/library/bnes/)

[NES / Famicom (Emux)](https://doc.libretro.com/library/emux_nes/)

[NES / Famicom (Nestopia UE)](https://doc.libretro.com/library/nestopia_ue/)

[NES / Famicom (QuickNES)](https://doc.libretro.com/library/quicknes/)

## License

GPLv2

## Extensions

*Content that can be loaded by the FCEUmm core have the following file extensions.*

fds|nes|unif|unf

## Database(s)

*RetroArch database(s) that are associated with the FCEUmm core*

* Nintendo - Nintendo Entertainment System

* Nintendo - Family Computer Disk System

## BIOS

*Required or optional firmware files go in RetroArch's system directory.*

|   Filename    |    Description                                                                |              md5sum              |
|:-------------:|:-----------------------------------------------------------------------------:|:--------------------------------:|
| disksys.rom   | Family Computer Disk System BIOS - Required for Famicom Disk System emulation | ca30b50f880eb660a320674ed365ef7a |
| nes.pal       | Custom NES Palette (Color Palette core option) - Optional                                                 |                                  |

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

The FCEUmm core's directory name is 'FCEUmm'

Game data is saved/loaded to and from where save files are stored.

Save states are saved/loaded to and from where state files are stored.

### Custom color palettes

To use custom color palettes in the FCEUmm core, the Color Palette core option must be set to custom and the custom color palette file you want to use must be in RetroArch's system directory. Make sure the custom palette file is named 'nes.pal'

Custom color palettes for the NES can be generated with either of these tools.

[Bisqwit's NTSC NES palette generator](http://bisqwit.iki.fi/utils/nespalette.php)

[Drag's NTSC NES palette generator](http://drag.wootest.net/misc/palgen.html)

## Core options

*The FCEUmm core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.*

- **Region Override** (**Auto**/NTSC/PAL/Dendy): Choose which region the system is from.
- **Preferred aspect ratio** (**8:7 PAR**/4:3): Choose the preferred aspect ratio. RetroArch's aspect ratio must be set to Core provided in the Video seetings.

??? note "Preferred aspect ratio - 8:7 PAR"
	![8by7_PAR](images\Cores\fceumm\8by7_PAR.png)
	
??? note "Preferred aspect ratio - 4:3"
	![4by3](images\Cores\fceumm\4by3.png)

- **Color Palette** (**default**/asqrealc/nintendo-vc/rgb/yuv-v3/unsaturated-final/sony-cxa2025as-us/pal/bmf-final2/bmf-final3/smooth-fbx/composite-direct-fbx/pvm-style-d93-fbx/ntsc-hardware-fbx/nes-classic-fbx-fs/nescap/wavebeam/raw/custom): Choose which color palette is going to be used.

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
- **Sound Volume** (**150**/160/170/180/190/200/210/220/230/240/250/0/10/20/30/40/50/60/70/80/90/100/110/120/130/140): Awaiting description.
- **Sound Quality** (**Low**/High/Very High): Awaiting description.
- **Swap Duty Cycles** (**Off**/On): Awaiting description.
- **Turbo Enable** (**None**/Player 1/Player 2/Both): Enable the use of the [Turbo B and Turbo A buttons](https://doc.libretro.com/library/fceumm/index.html#controllers-graph)
- **Turbo Delay (in frames)** (**3**/5/10/15/30/60/1/2): The number of frames between consecutive buttton presses when the Turbo B or Turbo A buttons are held down.
- **Zapper Mode** (**pointer**/mouse): Awaiting description.
- **Show Crosshair** (Off/**On**): Show the crosshair for the Zapper device type.

??? note "Show Crosshair - On"
	![show_crosshair_on](images\Cores\fceumm\show_crosshair_on.png)
	
??? note "Show Crosshair - Off"
	![show_crosshair_off](images\Cores\fceumm\show_crosshair_off.png)	

- **Overclocking** (**Off**/2x-Postrender/2x-VBlank): Awaiting description.

## Controllers

*The FCEUmm core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):*

### User 1 - 2 Device Type(s)

* **Auto** - *Depending on the loaded content, the core will automatically emulate a Gamepad and/or a Zapper*

* Gamepad - Joypad - [*Nintendo Entertainment System Controller*](http://nintendo.wikia.com/wiki/Nintendo_Entertainment_System_controller)

* Zapper - Mouse - [*Nintendo Entertainment System light gun accessory.*](http://nintendo.wikia.com/wiki/NES_Zapper)

### User 3 - 16 Device Type(s)

* **RetroPad** - Joypad

### Controllers graph

!!! warning ""
	In order to use the Turbo A and Turbo B buttons, the Turbo Enable core option must be set to on.

| FCEUmm                  | RetroPad                                               |
|-------------------------|--------------------------------------------------------|
| B                       | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)       |
| Turbo B                 | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)       |
| Select                  | ![RetroPad_Select](images/RetroPad/Retro_Select.png)   |
| Start                   | ![RetroPad_Start](images/RetroPad/Retro_Start.png)     |
| D-Pad Up                | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)    |
| D-Pad Down              | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)  |
| D-Pad Left              | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)  |
| D-Pad Right             | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png) |
| A                       | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)       |
| Turbo A                 | ![RetroPad_X](images/RetroPad/Retro_X_Round.png)       |
| (FDS) Disk Side Change  | ![RetroPad_L1](images/RetroPad/Retro_L1.png)           |
| (FDS) Insert/Eject Disk | ![RetroPad_R1](images/RetroPad/Retro_R1.png)           |
| (VSSystem) Insert Coin  | ![RetroPad_R2](images/RetroPad/Retro_R2.png)           |

| RetroMouse                                                      | Zapper    |
|-----------------------------------------------------------------|-----------|
| ![Retro_Mouse](images/RetroMouse/Retro_Mouse.png)               | Crosshair |
| ![Retro_Left](images/RetroMouse/Retro_Left.png)                 | Trigger   |

## Compatibility

| Game                         | Issue                                                        |
|------------------------------|--------------------------------------------------------------|
| Ms. Pac-Man (Tengen version) | Graphical glitches on the sides of the screen. (1)           |
| Skull & Crossbones           | Graphical glitches and screen shaking when in 2-player mode. | 

??? note "(1)"
	![mspacman_graphicalglitches](images\Cores\fceumm\mspacman_graphicalglitches.png)

## External Links

* [Libretro Repository](https://github.com/libretro/libretro-fceumm)
* [Report Core Issues Here](https://github.com/libretro/libretro-meta)
* [Official Website](http://cah4e3.shedevr.org.ru/fceultra.php)
* [Official Sourceforge Repository](https://sourceforge.net/projects/fceumm/)