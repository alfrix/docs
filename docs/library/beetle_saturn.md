# Sega Saturn (Beetle Saturn)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_saturn.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Port of standalone Mednafen Saturn to libretro.

### Why use this core?

Awaiting description.

### How to get and install the Beetle Saturn core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Sega Saturn (Beetle Saturn)'.

<center> ![](images\Cores\beetle_saturn\saturn.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

- If you are asked which core to select, choose 'Sega Saturn (Beetle Saturn)'.

The content should now start running!

### Authors

- [Mednafen Team](https://mednafen.github.io/)

## See also

### Saturn

- [Sega Saturn (Yabause)](https://docs.libretro.com/library/Yabause/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Beetle Saturn core is licensed under

- [GPLv2](https://github.com/libretro/beetle-saturn-libretro/blob/master/COPYING)

## Extensions

Content that can be loaded by the Beetle Saturn core have the following file extensions:

- .cue
- .toc
- .m3u
- .ccd
- .chd

## Databases

RetroArch database(s) that are associated with the Beetle Saturn core:

- [Sega - Saturn](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Saturn.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

|   Filename       |    Description                                                             |              md5sum              |
|:----------------:|:--------------------------------------------------------------------------:|:--------------------------------:|
| sega_101.bin     | Saturn JP BIOS - Required                                                  | 85ec9ca47d8f6807718151cbcca8b964 |
| mpr-17933.bin    | Saturn US/EU BIOS - Required                                               | 3240872c70984b6cbfda1586cab68dbe |
| mpr-18811-mx.ic1 | The King of Fighters '95 ROM Cartridge - Required for this game            | 255113ba943c92a54facd25a10fd780c |
| mpr-19367-mx.ic1 | Ultraman: Hikari no Kyojin Densetsu ROM Cartridge - Required for this game | 1cd19988d1d72a3e7caa0b73234c96b4 |

!!! attention
	The King of Fighters '95 and Ultraman: Hikari no Kyojin Densetsu ROM Cartridges can be manually selected with the ['Cartridge' core option](https://docs.libretro.com/library/beetle_saturn#core-options).

## Features

RetroArch-level settings or features that the Beetle Saturn core respects.

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
| RetroArch Cheats  | -         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | -         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| Softpatching      | ✕         |
| Disk Control      | ✔         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The Beetle Saturn core's directory name is 'Mednafen Saturn'

The Beetle Saturn core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.bcr (External cartridge backup save)
- 'content-name'.bkr (Internal save)
- 'content-name'.smpc (SMPC's emulated Real-Time Clock save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The Beetle Saturn core's internal FPS is 59.82
- The Beetle Saturn core's internal sample rate is 44100 Hz
- The Beetle Saturn core's core provided aspect ratio is 4/3

## Loading content

Beetle Saturn needs a cue-sheet that points to an image file. A cue sheet, or cue file, is a metadata file which describes how the tracks of a CD or DVD are laid out.

If you have e.g. `foo.bin`, you should create a text file and save it as `foo.cue`. If you're playing a single-track Saturn game, then the cue file contents should look like this:

`foobin.cue`
```
 FILE "foo.bin" BINARY
  TRACK 01 MODE1/2352
   INDEX 01 00:00:00
```

After that, you can load the `foo.cue` file in RetroArch with the Beetle Saturn core.

!!! attention
    Certain Saturn games are multi-track, so their .cue files might be more complicated.
	
## Multiple-disk games

If foo is a multiple-disk game, you should have .cue files for each one, e.g. `foo (Disc 1).cue`, `foo (Disc 2).cue`, `foo (Disc 3).cue`.

To take advantage of Beetle Saturn's Disk Control feature for disk swapping, an index file (a m3u file) should be made.

Create a text file and save it as `foo.m3u`. Then enter your game's .cue files on it. The m3u file contents should look something like this:

`foo.m3u`
```
foo (Disc 1).cue
foo (Disc 2).cue
foo (Disc 3).cue
```

After that, you can load the `foo.m3u` file in RetroArch with the Beetle Saturn core.

## Core options

The Beetle Saturn core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **System Region** (**Auto Detect**/Japan/North America/Europe/South Korea/Asia (NTSC)/Asia (PAL)/Brazil/Latin America)

<center> Choose which region the system is from. </center>

- **Cartridge** (**Auto Detect**/None/Backup Memory/Extended RAM (1MB)/Extended RAM (4MB)/The King of Fighters '95/Ultraman: Hikari no Kyojin Densetsu)

<center> For information regarding The King of Fighters '95 ROM Cartridge and the Ultraman: Hikari no Kyojin Densetsu ROM Cartridge, please look at the [BIOS section](https://docs.libretro.com/library/beetle_saturn#bios). </center>

- **6Player Adaptor on Port 1** (**Off**/On)

<center> Enable [multitap](https://segaretro.org/Saturn_6_Player_Adaptor) on Saturn port 1. </center>

- **6Player Adaptor on Port 2** (**Off**/On)

<center> Enable [multitap](https://segaretro.org/Saturn_6_Player_Adaptor) on Saturn port 2. </center>

- **3D Pad - Analog Deadzone** (0% to 30% in increments of 5%. **15% is default**)

<center> Configure the '3D Control Pad' Device Type's analog deadzone. </center>

- **3D Pad - Trigger Deadzone** (0% to 30% in increments of 5%. **15% is default**)

<center> Configure the '3D Control Pad' Device Type's trigger deadzone. </center>

- **Mouse - Sensitivity** (5% to 200% in increments of 5%. **100% is default**)

<center> Configure the 'Mouse' device type's sensitivity. </center>

- **Gun - Crosshair** (**Cross**/Dot/Off)

<center> Choose the crosshair for the 'Stunner' and 'Virtua Gun' device types. Setting it to Off disables the crosshair. </center>

??? note "Gun - Crosshair - Cross"
	![](images\Cores\beetle_saturn\cross.png)
	
??? note "Gun - Crosshair - Dot"
	![](images\Cores\beetle_saturn\dot.png)

??? note "Gun - Crosshair - Off"
	![](images\Cores\beetle_saturn\off.png)	

- **CD Image Cache (restart)** (**Off**/On)

<center> Loads the complete image in memory at startup. Can potentially decrease loading times at the cost of increased startup time. </center>

- **Automatically set RTC on game load** (Off/**On**)

<center> Automatically set the SMPC's emulated Real-Time Clock to the host system's current time and date upon game load. </center>

- **BIOS language** (**english**/german/french/spanish/italian/japanese)

<center> Self explanatory. Also affects language used in some games (e.g. the European release of "Panzer Dragoon"). </center>

- **Horizontal Overscan Mask** (0 to 60 in increments of 2. **0 is default**)

<center> Self-explanatory. </center>

- **Initial scanline** (0 to 40 in increments of 1. **0 is default**)

<center> Adjust the first displayed scanline in NTSC mode. </center>

- **Last scanline** (210 to 239 in increments of 1. **239 is default**)

<center> Adjust the first displayed scanline in PAL mode. </center>

- **Initial scanline PAL** (0 to 60 in increments of 1. **16 is default**)

<center> Adjust the last displayed scanline in NTSC mode. </center>

- **Last scanline PAL** (230 to 287 in increments of 1. **271 is default**)

<center> Adjust the last displayed scanline in PAL mode. </center>

- **Enable Horizontal Blend(blur)** (**Off**/On)

<center> Self-explanatory. </center>

??? note "Enable Horizontal Blend(blur) - Off"
	![](images\Cores\beetle_saturn\blend_off.png)
	
??? note "Enable Horizontal Blend(blur) - On"
	![](images\Cores\beetle_saturn\blend_on.png)

## Controllers

### Device types

The Beetle Saturn core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 12 device types

- None - Input disabled.
- [**Control Pad**](http://segaretro.org/Control_Pad_(Saturn)) - Joypad
- [3D Control Pad](http://segaretro.org/3D_Control_Pad) - Analog
- [Arcade Racer](http://segaretro.org/Arcade_Racer_Joystick) - Analog
- [Mission Stick](https://segaretro.org/Sega_Mission_Stick) - Analog
- [Mouse](http://segaretro.org/Shuttle_Mouse) - Mouse
- [Stunner](http://segaretro.org/Virtua_Gun) - Lightgun
- [Twin-Stick](https://segaretro.org/Saturn_Twin-Stick) - Analog
- [Virtua Gun](https://segaretro.org/Virtua_Gun) - Lightgun
- [Dual Mission Sticks](https://segaretro.org/Sega_Mission_Stick) - Analog - Panzer Dragoon Zwei only

### Multitap support

Activating multitap support in compatible games can be configured by the ['6Player Adaptor on Port 1' and '6Player Adaptor on Port 2' core options](https://docs.libretro.com/library/beetle_saturn#core-options).

### Controller tables

#### Joypad and analog device type table

| User 1 - 12 Input descriptors | RetroPad Inputs                              | Control Pad  | 3D Control Pad | Arcade Racer              | Mission Stick  | Twin-Stick          | Dual Mission Sticks  |
|-------------------------------|----------------------------------------------|--------------|----------------|---------------------------|----------------|---------------------|----------------------|
| A Button                      | ![](images/RetroPad/Retro_B_Round.png)       | A Button     | A Button       | A Button                  | A Button       |                     | A Button             |
| X Button                      | ![](images/RetroPad/Retro_Y_Round.png)       | X Button     | X Button       | X Button                  | X Button       |                     | X Button             |
| Mode Switch                   | ![](images/RetroPad/Retro_Select.png)        |              | Mode Switch    |                           |                |                     |                      |
| Start Button                  | ![](images/RetroPad/Retro_Start.png)         | Start Button | Start Button   | Start Button              | Start Button   | Start Button        | Start Button         |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up     | D-Pad Up       |                           |                |                     |                      |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down   | D-Pad Down     |                           |                |                     |                      |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left   | D-Pad Left     |                           |                |                     |                      |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right  | D-Pad Right    |                           |                |                     |                      |
| B Button                      | ![](images/RetroPad/Retro_A_Round.png)       | B Button     | B Button       | B Button                  | B Button       |                     | B Button             |
| Y Button                      | ![](images/RetroPad/Retro_X_Round.png)       | Y Button     | Y Button       | Y Button                  | Y Button       |                     | Y Button             |
| Z Button                      | ![](images/RetroPad/Retro_L1.png)            | Z Button     | Z Button       | Z Button                  | Z Button       | Left Stick Button   | Z Button             |
| C Button                      | ![](images/RetroPad/Retro_R1.png)            | C Button     | C Button       | C Button                  | C Button       | Right Stick Button  | C Button             |
| L Button                      | ![](images/RetroPad/Retro_L2.png)            | L Button     | L Button       | Left shift paddle (Up)    | L Button       | Left Stick Trigger  | L Button             |
| R Button                      | ![](images/RetroPad/Retro_R2.png)            | R Button     | R Button       | Right shift paddle (Down) | R Button       | Right Stick Trigger | R Button             |
|                               | ![](images/RetroPad/Retro_R3.png)            |              |                |                           | Throttle latch |                     | Throttle latch       |
| Analog X                      | ![](images/RetroPad/Retro_Left_Stick.png) X  |              | Analog X       | Analog wheel              | Analog Stick X | Left Stick X        | Left Analog Stick X  |
| Analog Y                      | ![](images/RetroPad/Retro_Left_Stick.png) Y  |              | Analog Y       |                           | Analog Stick Y | Left Stick Y        | Left Analog Stick Y  |
| Analog X (Right)              | ![](images/RetroPad/Retro_Right_Stick.png) X |              |                |                           |                | Right Stick X       | Right Analog Stick X |
| Analog Y (Right)              | ![](images/RetroPad/Retro_Right_Stick.png) Y |              |                |                           | Throttle       | Right Stick Y       | Right Analog Stick Y |

#### Mouse device type table

| User 1 - 12 Input descriptors | RetroMouse Inputs                        | Mouse              |
|-------------------------------|------------------------------------------|--------------------|
|                               | ![](images/RetroMouse/Retro_Mouse.png)   | Mouse cursor       |
|                               | ![](images/RetroMouse/Retro_Left.png)    | A                  |
|                               | ![](images/RetroMouse/Retro_Right.png)   | B                  |
|                               | ![](images/RetroMouse/Retro_Middle.png)  | C                  |
|                               | Mouse Button 4                           | Start              |
|                               | Mouse Button 5                           | Start              |

#### Lightgun device type table

| User 1 - 12 Input descriptors | RetroLightgun Inputs | Stunner            | Virtua Gun         |
|-------------------------------|----------------------|--------------------|--------------------|
|                               | Gun                  | Stunner cursor     | Virtua Gun cursor  |
|                               | Gun Trigger          | Stunner trigger    | Virtua Gun trigger |
|                               | Gun Reload           | Stunner reload     | Virtua Gun reload  |
|                               | Gun Start            | Stunner start      | Virtua Gun start   |

## Compatibility

Awaiting description.

## External Links

- [Libretro Beetle Saturn Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_saturn_libretro.info)
- [Libretro Beetle Saturn Github Repository](https://github.com/libretro/beetle-saturn-libretro)
- [Report Libretro Beetle Saturn Core Issues Here](https://github.com/libretro/beetle-saturn-libretro/issues)
- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)