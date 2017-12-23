# PC Engine SuperGrafx (Beetle SGX)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_sgx.md). Changes are proposed using "Pull Requests."

There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)

You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).

## Background

Standalone port of Mednafen PCE Fast to libretro. This one only emulates a SuperGrafx TG-16

### Why use this core?

Awaiting description.

### How to get and install the Beetle SGX core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'PC Engine SuperGrafx (Beetle SGX)'.

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'PC Engine SuperGrafx (Beetle SGX)'.

The content should now start running!

### Authors

- [Mednafen Team](https://mednafen.github.io/)

## See also

### NEC PC Engine

- [PC Engine/PCE-CD (Beetle PCE FAST)](https://docs.libretro.com/library/beetle_pce_fast/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

[GPLv2](https://github.com/libretro/beetle-supergrafx-libretro/blob/master/COPYING)

## Extensions

Content that can be loaded by the Beetle SGX core have the following file extensions:

- .pce
- .sgx
- .cue
- .ccd
- .chd

## Databases

RetroArch database(s) that are associated with the Beetle SGX core:

- [NEC - PC Engine SuperGrafx](https://github.com/libretro/libretro-database/blob/master/rdb/NEC%20-%20PC%20Engine%20SuperGrafx.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

|   Filename    |    Description                        |              md5sum              |
|:-------------:|:-------------------------------------:|:--------------------------------:|
| syscard3.pce  | Super CD-ROM2 System V3.xx - Required | 38179df8f4ac870017db21ebcbf53114 |
| syscard2.pce  | CD-ROM System V2.xx - Optional        |                                  |
| syscard1.pce  | CD-ROM System V1.xx - Optional        |                                  |
| gexpress.pce  | Game Express CD Card - Optional       |                                  |

!!! attention
	Which BIOS file the Beetle SGX core will use can be configured by the ['CD BIOS' core option](https://docs.libretro.com/library/beetle_sgx#core-options).

## Features

RetroArch-level settings or features that the Beetle SGX core respects.

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
| Softpatching      | ✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The Beetle SGX core's directory name is 'Mednafen SuperGrafx'

The Beetle SGX core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The Beetle SGX core's internal FPS is 59.82
- The Beetle SGX core's internal sample rate is 44100 Hz
- The Beetle SGX core's core provided aspect ratio is dependent on the ['Aspect Ratio' core option](https://docs.libretro.com/library/beetle_sgx#core-options).

## Loading PC Engine CD content

To load PC Engine CD content, Beetle SGX needs a cue-sheet that points to an image file. A cue sheet, or cue file, is a metadata file which describes how the tracks of a CD or DVD are laid out.

If you have e.g. `foo.bin`, you should create a text file and save it as `foo.cue`. If you're playing a single-track Saturn game, then the cue file contents should look like this:

`foobin.cue`
```
 FILE "foo.bin" BINARY
  TRACK 01 MODE1/2352
   INDEX 01 00:00:00
```

After that, you can load the `foo.cue` file in RetroArch with the Beetle SGX core.

!!! warning ""
    Certain PC Engine content are multi-track, so their .cue files might be more complicated.

## Core options

The Beetle SGX core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **CD Image Cache (Restart)** (**Off**/On) 

<center> Loads the complete image in memory at startup. </center>

- **CD Bios (Restart)** (**System Card 3**/Games Express/System Card 1/System Card 2)

<center> Select which CD BIOS to use. </center>

- **Force SuperGrafx Emulation (Restart)** (**Off**/On)

<center> Awaiting description. </center>

- **No Sprite Limit (Restart)** (**Off**/On)

<center> Self-explanatory. </center>

- **CPU Overclock Multiplier (Restart)** (**1**/2/3/4/5/6/7/8/9/10/20/30/40/50)

<center> Awaiting description. </center>

- **Horizontal Overscan (352 Width Mode Only)** (300 to 352 in increments of 2. **352 in default**.)

<center> Awaiting description. </center>

- **Initial scanline** (0 to 40 in increments of 1. **3 is default.**)

<center> Adjust first display scanline. </center>

- **Last scanline** (208 to 242 in increments of 1. **242 is default.**)

<center> Adjust last display scanline. </center>

- **(CD) CDDA Volume %** (0 to 200 in increments of 10. **100 is default**.)

<center> Awaiting description. </center>

- **(CD) ADPCM Volume %** (0 to 200 in increments of 10. **100 is default**.)

<center> Awaiting description. </center>

- **(CD) CD PSG Volume %** (0 to 200 in increments of 10. **100 is default**.)

<center> Awaiting description. </center>

- **(CD) CD Speed** (**1**/2/4/8)

<center> Set the speed of the emulated CD drive. </center>

- **Turbo Delay** (**3**/4/5/6/7/8/9/10/11/12/13/14/15/30/60/2)

<center> Awaiting description. </center>

- **Turbo ON/OFF Toggle** (**Off**/On)

<center> Look at the [Controllers table section](https://docs.libretro.com/library/beetle_sgx#Controllers-tables) for more information. </center>

- **Alternate Turbo Hotkey** (**Off**/On)

<center> Look at the [Controllers table section](https://docs.libretro.com/library/beetle_sgx#Controllers-tables) for more information.  </center>

- **Aspect Ratio** (**auto**/6:5/4:3)

<center> Configure the core provided aspect ratio.. </center>

## Controllers

### Device types

The Beetle SGX core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 2 device types

- None - Doesn't disable input.
- **PCE Joypad** - Joypad
- Mouse - Mouse

### Controller tables

#### Joypad and analog device type table

| User 1 - 5 Input descriptors  | RetroPad Inputs                              | PCE Joypad 2-button mode  | PCE Joypad 6-button mode |
|-------------------------------|----------------------------------------------|---------------------------|--------------------------|
| II                            | ![](images/RetroPad/Retro_B_Round.png)       | II                        | II                       |
| III                           | ![](images/RetroPad/Retro_Y_Round.png)       | II Turbo On/Off           | III                      |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select                    | Select                   |
| Run                           | ![](images/RetroPad/Retro_Start.png)         | Run                       | Run                      |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up                  | D-Pad Up                 |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down                | D-Pad Down               |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left                | D-Pad Left               |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right               | D-Pad Right              |
| I                             | ![](images/RetroPad/Retro_A_Round.png)       | I                         | I                        |
| IV                            | ![](images/RetroPad/Retro_X_Round.png)       | I Turbo On/Off            | IV                       |
| V                             | ![](images/RetroPad/Retro_L1.png)            |                           | V                        |
| VI                            | ![](images/RetroPad/Retro_R1.png)            |                           | VI                       |
| Mode Switch                   | ![](images/RetroPad/Retro_L2.png)            | Mode Switch               | Mode Switch              |
|                               | ![](images/RetroPad/Retro_L3.png)            | Alternate II Turbo On/Off |                          |
|                               | ![](images/RetroPad/Retro_R3.png)            | Alternate I Turbo On/Off  |                          |

!!! attention
	Which PCE Joypad button mode is in use can be configured by the Mode Switch input.
	
!!! attention
	The regular Turbo inputs for 2-button mode are only active when the ['Turbo ON/OFF Toggle' core option](https://docs.libretro.com/library/beetle_sgx#core-options) is set to On.
	
!!! attention
	The Alternate Turbo inputs for 2-button mode are only active when the ['Turbo ON/OFF Toggle' core option](https://docs.libretro.com/library/beetle_sgx#core-options) is set to On and the ['Alternate Turbo Hotkey' core option](https://docs.libretro.com/library/beetle_sgx#core-options) is set to On.

#### Mouse device type table

| User 1 - 2 Input descriptors  | RetroMouse Inputs                        | Mouse              |
|-------------------------------|------------------------------------------|--------------------|
|                               | ![](images/RetroMouse/Retro_Mouse.png)   | -                  |
|                               | ![](images/RetroMouse/Retro_Left.png)    | -                  |
|                               | ![](images/RetroMouse/Retro_Right.png)   | -                  |

## Compatibility

Awaiting description.

## External Links

- [Libretro Beetle SGX Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_supergrafx_libretro.info)
- [Libretro Beetle SGX Github Repository](https://github.com/libretro/beetle-supergrafx-libretro)
- [Report Libretro Beetle SGX Core Issues Here](https://github.com/libretro/beetle-supergrafx-libretro/issues)
- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)