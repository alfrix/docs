# SNES / Super Famicom (nSide Balanced)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/nside_balanced.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

A fork of higan v106 that reimplements the Balanced profile.

### Why use this core?

Awaiting description.

### How to get and install the nSide Balanced core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'SNES / Super Famicom (nSide Balanced)'.

<center> ![](images\Cores\higan\nside_balanced.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\snes.png) </center>

- If you are asked which core to select, choose 'SNES / Super Famicom (nSide Balanced)'.

The content should now start running!

### Authors

- hex-usr

## See also

### SNES

- [SNES / Super Famicom (Beetle bsnes)](https://docs.libretro.com/library/beetle_snes/)
- [SNES / Super Famicom (bsnes Accuracy)](https://docs.libretro.com/library/bsnes_accuracy/)
- [SNES / Super Famicom (bsnes Balanced)](https://docs.libretro.com/library/bsnes_balanced/)
- [SNES / Super Famicom (bsnes C++98 (v085))](https://docs.libretro.com/library/bsnes_cplusplus98/)
- [SNES / Super Famicom (bsnes Performance)](https://docs.libretro.com/library/bsnes_performance/)
- [SNES / Super Famicom (bsnes-mercury Accuracy)](https://docs.libretro.com/library/bsnes_mercury_accuracy/)
- [SNES / Super Famicom (bsnes-mercury Balanced)](https://docs.libretro.com/library/bsnes_mercury_balanced/)
- [SNES / Super Famicom (bsnes-mercury Performance)](https://docs.libretro.com/library/bsnes_mercury_performance/)
- [SNES / Super Famicom (higan Accuracy)](https://docs.libretro.com/library/higan_accuracy/)
- [SNES / Super Famicom (Snes9x 2002)](https://docs.libretro.com/library/snes9x_2002/)
- [SNES / Super Famicom (Snes9x 2005 Plus)](https://docs.libretro.com/library/snes9x_2005_plus/)
- [SNES / Super Famicom (Snes9x 2005)](https://docs.libretro.com/library/snes9x_2005/)
- [SNES / Super Famicom (Snes9x 2010)](https://docs.libretro.com/library/snes9x_2010/)
- [SNES / Super Famicom (Snes9x)](https://docs.libretro.com/library/snes9x/)

### GB/GBC

- [Game Boy / Game Boy Color (Emux GB)](https://docs.libretro.com/library/emux_gb/)
- [Game Boy / Game Boy Color (Gambatte)](https://docs.libretro.com/library/gambatte/)
- [Game Boy / Game Boy Color (SameBoy)](https://docs.libretro.com/library/sameboy/)
- [Game Boy / Game Boy Color (TGB Dual)](https://docs.libretro.com/library/tgb_dual/)
- [Game Boy / Game Boy Color (Gearboy)](https://docs.libretro.com/library/gearboy/)
- [Game Boy Advance (mGBA)](https://docs.libretro.com/library/mgba/)
- [SNES / Super Famicom (higan Accuracy)](https://docs.libretro.com/library/higan_accuracy/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The nSide Balanced core is licensed under

- [GPLv3](https://github.com/hex-usr/nSide/blob/master/gpl-3.0.txt)

## Extensions

Content that can be loaded by the nSide Balanced core have the following file extensions:

- .sfc
- .smc
- .gb
- .gbc
- .bml
- .rom

## Databases

RetroArch database(s) that are associated with the nSide Balanced core:

- [Nintendo - Super Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System%20Hacks.rdb)
- [Nintendo - Super Nintendo Entertainment System Hacks](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System%20Hacks.rdb)
- [Nintendo - Game Boy](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy.rdb)
- [Nintendo - Game Boy Color](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Color.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

!!! attention
	nSide Balanced uses split ROMS for special chip games.
	
Notable DSP1/DSP1B Games:

- Super Mario Kart
- Pilotwings

Notable DSP2 Games:

- Dungeon Master

Notable DSP3 Games:

- SD Gundam GX

Notable DSP4 Games:

- Top Gear 3000

Notable Cx4 Games:

- Mega Man X2
- Mega Man X3

|   Filename             |    Description                         |              md5sum              |
|:----------------------:|:--------------------------------------:|:--------------------------------:|
| dsp1.data.rom          | DSP1 co-processor firmware - Optional  | 3d81b45fa0c2aa8b852dfb1ece7c0971 |
| dsp1.program.rom       | DSP1 co-processor firmware - Optional  | ae209fbe789fbf11a48aea5ab1197321 |
| dsp1b.data.rom         | DSP1B co-processor firmware - Optional | 1e3f568634a7d8284020dddc0ae905bc |
| dsp1b.program.rom      | DSP1B co-processor firmware - Optional | d10f446888e097cbf500f3f663cf4f6d |
| dsp2.data.rom          | DSP2 co-processor firmware - Optional  | e9417e29223b139c3c4b635a2a3b8744 |
| dsp2.program.rom       | DSP2 co-processor firmware - Optional  | aa6e5922a3ed5ded54f24247c11143c5 |
| dsp3.data.rom          | DSP3 co-processor firmware - Optional  | 0a81210c0a940b997dd9843281008ee6 |
| dsp3.program.rom       | DSP3 co-processor firmware - Optional  | d99ca4562818d49cee1f242705bba6f8 |
| dsp4.data.rom          | DSP4 co-processor firmware - Optional  | ee4990879eb68e3cbca239c5bc20303d |
| dsp4.program.rom       | DSP4 co-processor firmware - Optional  | a151023b948b90ffc23a5b594bb6fef2 |
| cx4.data.rom           | CX4 co-processor firmware - Optional   | 037ac4296b6b6a5c47c440188d3c72e3 |
| st010.data.rom         | ST010 co-processor firmware - Optional | 254d70762b6f59f99c27c395aba7d07d |
| st010.program.rom      | ST010 co-processor firmware - Optional | 1d70019179a59a566a0bb5d3f2845544 |
| st011.data.rom         | ST011 co-processor firmware - Optional | 10bd3f4aa949737ab9836512c35bcc29 |
| st011.program.rom      | ST011 co-processor firmware - Optional | 95222ebf1c0c2990bcf25db43743f032 |
| st018.data.rom         | ST018 co-processor firmware - Optional | 49c898b60d0f15e90d0ba780dd12f366 |
| st018.program.rom      | ST018 co-processor firmware - Optional | dda40ccd57390c96e49d30a041f9a9e7 |
| SGB1.sfc/sgb1.boot.rom | Super Game Boy BIOS - Optional         |                                  |
| SGB1.sfc/program.rom   | Super Game Boy ROM - Optional          |                                  |
| SGB2.sfc/sgb2.boot.rom | Super Game Boy 2 BIOS - Optional       |                                  |
| SGB2.sfc/program.rom   | Super Game Boy 2 ROM - Optional        |                                  |

!!! attention
	Firmware files for SGB emulation need to be in directories called SGB1.sfc and SGB2.sfc in RetroArch's system directory. Look at the [Super GameBoy support section](https://docs.libretro.com/library/nside_balanced#super-gameboy-support) for more information.

## Features

RetroArch-level settings or features that the nSide Balanced core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| Core Options      | ✔         |
| RetroAchievements | ✕         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | -         |
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

The nSide Balanced core's directory name is 'higan (Super Famicom Balanced)'

The nSide Balanced core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The nSide Balanced core's internal FPS is (FPS)
- The nSide Balanced core's internal sample rate is (Rate)
- The nSide Balanced core's core provided aspect ratio is (Ratio)

### Super Gameboy Support

The nSide Balanced core uses a simplified Super Game Boy routine that makes it much easier to access this feature than with the old v094-based cores. 

Instead of using the complex, CLI-based 'subsystem' launch commands, it looks for the necessary files in the system/BIOS directory whenever you feed the core a *.gb/c file.

To get it working, you'll need one or more Super Game Boy ROMs and the sgb.boot.rom BIOS.

**Step 1**

Make 2 subdirectories in RetroArch's system directory, one named SGB1.sfc and the other named SGB2.sfc.

**Step 2**

Copy your original Super Game Boy ROM into the SGB1.sfc directory and then rename it to program.rom. Copy your Super Game Boy 2 ROM into the SGB2.sfc directory and then rename it program.rom, as well.

**Step 3**

Copy your sgb.boot.rom BIOS into each of your SGB1.sfc and SGB2.sfc directories, and rename them to sgb1.boot.rom and sgb2.boot.rom, respectively. 

The ['Preferred Super GameBoy BIOS' core option](https://docs.libretro.com/library/nside_balanced#core-options) lets you choose which of the two SGB BIOSes to use.

**Step 4**

Load a SGB-supported GB/GBC rom.

**Done**

![](images/Cores/higan/sgb.png)

!!! warning
	There may be graphical glitches when Rewind is set to On in RetroArch's settings.

### MSU-1 Support

Awaiting description.

## Core options

The nSide Balanced core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Internal resolution** (**512x480**/512x448/512x240/512x224/256x240/256x224)

<center> Self-explanatory. </center>

??? note "512x480"
    ![](images/Cores/higan/512x480.png)

??? note "512x448"
    ![](images/Cores/higan/512x448.png)

??? note "512x240"
    ![](images/Cores/higan/512x240.png)

??? note "512x224"
    ![](images/Cores/higan/512x224.png)

??? note "256x240"
    ![](images/Cores/higan/256x240.png)

??? note "256x224"
    ![](images/Cores/higan/256x224.png)

- **Color emulation** (**Off**/On)

<center> Simulates the way a console’s display device differs from modern computer monitor’s colour reproduction. In particular, it simulates the slightly-different gamma correction used by the Super Famicom. </center>

??? note "Color emulation - Disabled"
    ![](images/Cores/higan/color_off.png)

??? note "Color emulation - Enabled"
    ![](images/Cores/higan/color_on.png)

- **Blur emulation**  (**Off**/On)

<center> Simulates the limited horizontal resolution of standard-definition TVs by blurring together horizontally-adjacent pixels. Games like Jurassic Park for the Super Famicom depend on this to emulate a transparency effect. </center>

??? note "Blur emulation - Disabled"
    ![](images/Cores/higan/blur_off.png)

??? note "Blur emulation - Enabled"
    ![](images/Cores/higan/blur_on.png)

- **Scanline emulation** (**Off**/On)

<center> Currently does not function properly </center>

- **Preferred Super GameBoy BIOS (restart)** (**SGB1.sfc/**/SGB2.sfc/)

<center> Choose what Super GameBoy BIOS you want to use. Look at the [Super GameBoy Support section](https://docs.libretro.com/library/nside_balanced#super-gameboy-support) for more information. </center>

## Controllers

### Device types

The nSide Balanced core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Input disabled.
- [**SNES Joypad**](http://nintendo.wikia.com/wiki/Super_Nintendo_Entertainment_System_controller) - Joypad
- [SNES Mouse](https://en.wikipedia.org/wiki/Super_NES_Mouse) - Mouse

#### User 2 device types

- None - Input disabled.
- [**SNES Joypad**](http://nintendo.wikia.com/wiki/Super_Nintendo_Entertainment_System_controller) - Joypad
- [SNES Mouse](https://en.wikipedia.org/wiki/Super_NES_Mouse) - Mouse
- [Multitap](http://nintendo.wikia.com/wiki/Super_Multitap) - Joypad - Allows for up to five players to play together in certain games.
- [SuperScope](https://en.wikipedia.org/wiki/Super_Scope) - Lightgun
- [Justifier](https://en.wikipedia.org/wiki/Konami_Justifier) - Lightgun
- [Justifiers](https://en.wikipedia.org/wiki/Konami_Justifier) - Lightgun - Two Justifiers are plugged in, for two-player Justifier games.

### Multitap support

Activating multitap support in compatible games can be configured by switching to the [Multitap device type](https://docs.libretro.com/library/nside_balanced#controllers) for User 2.

### Controller tables

#### Joypad and analog device type table

| User 1 - 5 Input descriptors  | RetroPad Inputs                              | SNES Joypad / Multitap |
|-------------------------------|----------------------------------------------|------------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                      |
| Y                             | ![](images/RetroPad/Retro_Y_Round.png)       | Y                      |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select                 |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start                  |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up               |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down             |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Lef              |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right            |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | A                      |
| X                             | ![](images/RetroPad/Retro_X_Round.png)       | X                      |
| L                             | ![](images/RetroPad/Retro_L1.png)            | L                      |
| R                             | ![](images/RetroPad/Retro_R1.png)            | R                      |

#### Mouse device type table

| User 1 - 2 Input descriptors  | RetroMouse Inputs                        | SNES Mouse              |
|-------------------------------|------------------------------------------|-------------------------|
|                               | ![](images/RetroMouse/Retro_Mouse.png)   | SNES Mouse Cursor       |
|                               | ![](images/RetroMouse/Retro_Left.png)    | SNES Mouse Left Button  |
|                               | ![](images/RetroMouse/Retro_Right.png)   | SNES Mouse Right Button |

#### Lightgun device type table

| User 2 Input descriptors      | RetroLightgun Inputs | SuperScope           | Justifier(s)        |
|-------------------------------|----------------------|----------------------|---------------------|
|                               | Gun                  | SuperScope Crosshair | Justifier Crosshair |
|                               | Gun Trigger          | SuperScope Trigger   | Justifier Trigger   |
|                               | Gun Cursor           | SuperScope Cursor    |                     |
|                               | Gun Turbo            | SuperScope Turbo     | Justifier Offscreen |
|                               | Gun Pause            | SuperScope Pause     | Justifier Start     |

!!! attention
	All of the Super Scope games made by Nintendo have a soft-reset to the game's main title. This is accomplished by pausing the game, then, while holding Cursor, the Fire button must be pressed twice.

## Compatibility

| Game                     | Issue                                                                          |
|--------------------------|--------------------------------------------------------------------------------|
| A.S.P. Air Strike Patrol | Black lines show up during gameplay. The shadow below the aircraft is missing. |

Incompatible with ROM hacks made to take advantage of emulator quirks, much like real hardware.

## External Links

- [Libretro nSide Balanced Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/higan_sfc_balanced_libretro.info)
- [Libretro nSide Balanced Github Repository](https://github.com/hex-usr/nSide)
- [Report Libretro nSide Balanced Core Issues Here](https://github.com/libretro/libretro-meta/issues)
- [Official higan Website](https://byuu.org/)
- [Official higan Upstream Downloads](https://byuu.org/emulation/higan/)