# PC-FX (Beetle PC-FX)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_pc_fx.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Beetle PC-FX is a port of Mednafen PC-FX video game system emulator for the NEC PC-FX.

### Why use this core?

Awaiting description.

### How to get and install the Beetle PC-FX core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'PC-FX (Beetle PC-FX)'.

<center> ![](images\Cores\beetle_pc_fx\beetle_pc_fx.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\screenshot_name.png) </center>

- If you are asked which core to select, choose 'PC-FX (Beetle PC-FX)'.

The content should now start running!

### Authors

- [Mednafen Team](https://mednafen.github.io/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Beetle PC-FX core is licensed under

- [GPLv2](https://github.com/libretro/beetle-pcfx-libretro/blob/master/COPYING)

## Extensions

Content that can be loaded by the Beetle PC-FX core have the following file extensions:

- .cue
- .ccd
- .toc
- .chd

## Databases

RetroArch database(s) that are associated with the Beetle PC-FX core:

- [NEC - PC-FX](https://github.com/libretro/libretro-database/blob/master/rdb/NEC%20-%20PC-FX.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

|   Filename    |    Description                           |              md5sum              |
|:-------------:|:----------------------------------------:|:--------------------------------:|
| pcfx.rom      | PC-FX BIOS v1.00 - 2 Sep 1994 - Required | 08e36edbea28a017f79f8d4f7ff9b6d7 |

## Features

RetroArch-level settings or features that the Beetle PC-FX core respects.

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
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | ✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✔         |

### Directories

The Beetle PC-FX core's directory name is 'Mednafen PC-FX'

The Beetle PC-FX core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Save)

**RetroArch's State directory**

- 'content-name-.state# (State)

### Geometry and timing

- The Beetle PC-FX core's internal FPS is 60
- The Beetle PC-FX core's internal sample rate is 44100 Hz
- The Beetle PC-FX core's core provided aspect ratio is 4/3

### Loading content

Beetle PC-FX needs a cue-sheet that points to an image file. A cue sheet, or cue file, is a metadata file which describes how the tracks of a CD or DVD are laid out.

If you have e.g. `foo.bin`, you should create a text file and save it as `foo.cue`. If you're playing a single-track Saturn game, then the cue file contents should look like this:

`foobin.cue`
```
 FILE "foo.bin" BINARY
  TRACK 01 MODE1/2352
   INDEX 01 00:00:00
```

After that, you can load the `foo.cue` file in RetroArch with the Beetle PC-FX core.

!!! attention
    Certain PC-FX games are multi-track, so their .cue files might be more complicated.
	
## Core options

The Beetle PC-FX core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **High Dotclock Width (Restart) (**1024**/256/341)

 Emulated width for 7.16MHz dot-clock mode. Lower values are faster, but will cause some degree of pixel distortion.

- **Suppress Channel Reset Clicks (Restart)** (Off/**On**)

 Hack to suppress clicks caused by forced channel resets.

- **Emulate Buggy Codec (Restart)** (**Off**/On)

 Hack that emulates the codec a buggy ADPCM encoder used for some games' ADPCM.

- **Sound Quality (Restart)** (**3**/4/5/0/1/2)

 Higher values correspond to better SNR and better preservation of higher frequencies("brightness"), at the cost of increased computational complexity and a negligible increase in latency.

- **Chroma channel bilinear interpolation  (Restart)** (**Off**/On)

 Enable bilinear interpolation on the chroma channel of RAINBOW YUV output. Enabling it may cause graphical glitches with some games.

- **No Sprite Limit (Restart)** (**Off**/On)

 Remove 16-sprites-per-scanline hardware limit.

- **Initial scanline** (0 to 40 in increments of 1. **4 is default**.)

 Adjust first display scanline.

- **Last scanline** (208 to 238 in increments of 1. **235 is default**.)

 Adjust last display scanline.

- **Mouse Sensitivity** (1.00 to 5.00 in increments of 0.25. **1.25 is default**.)

 Configure the sensitivity of the 'PCFX Mouse' device type,

## Controllers

### Device types

The Beetle PC-FX core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 2 device types

- None - Doesn't disable input.
- **PCFX Joypad** - Joypad
- PCFX Mouse - Mouse

### Controller tables

#### Joypad and analog device type table

| User 1 - 6 Remap descriptors  | RetroPad Inputs                              | PCFX Joypad        |
|-------------------------------|----------------------------------------------|--------------------|
| II                            | ![](images/RetroPad/Retro_B_Round.png)       | II                 |
| IV                            | ![](images/RetroPad/Retro_Y_Round.png)       | IV                 |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select             |
| Run                           | ![](images/RetroPad/Retro_Start.png)         | Run                |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up           |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down         |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left         |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right        |
| I                             | ![](images/RetroPad/Retro_A_Round.png)       | I                  |
| III                           | ![](images/RetroPad/Retro_X_Round.png)       | III                |
| V                             | ![](images/RetroPad/Retro_L1.png)            | V                  |
| VI                            | ![](images/RetroPad/Retro_R1.png)            | VI                 |
| MODE 1 (Switch)               | ![](images/RetroPad/Retro_L2.png)            | MODE 1 (Switch)    |
| MODE 2 (Switch)               | ![](images/RetroPad/Retro_R2.png)            | MODE 2 (Switch)    |

#### Mouse device type table

| User # Remap descriptors      | RetroMouse Inputs                        | PCFX Mouse              |
|-------------------------------|------------------------------------------|-------------------------|
|                               | ![](images/RetroMouse/Retro_Mouse.png)   | PCFX Mouse Cursor       |
|                               | ![](images/RetroMouse/Retro_Left.png)    | PCFX Mouse Left Button  |
|                               | ![](images/RetroMouse/Retro_Right.png)   | PCFX Mouse Right Button |

## Compatibility

| Game                                                                | Issue                                                   |
|---------------------------------------------------------------------|---------------------------------------------------------|
| Pia Carrot e Youkoso!! (Japan) [T-En by David Michel + filler v1.0] | Doesn't boot. Confirmed to work on real hardware.       |

## External Links

- [Libretro Beetle PC-FX Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_pcfx_libretro.info)
- [Libretro Beetle PC-FX Github Repository](https://github.com/libretro/beetle-pcfx-libretro)
- [Report Libretro Beetle PC-FX Core Issues Here](https://github.com/libretro/beetle-pcfx-libretro/issues)
- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)