# Sega Saturn (Beetle Saturn)

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_saturn.md). Changes are proposed using "Pull Requests."

## Background

Port of standalone Mednafen Saturn to libretro.

### Why use this core?

Awaiting description.

### How to get and install the Beetle Saturn core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Sega Saturn (Beetle Saturn)'.

After this has finished downloading, the core should now be ready for use!

### Authors

- Mednafen Team

## See also

- [Sega Saturn (Yabause)](https://buildbot.libretro.com/.docs/library/Yabause/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://buildbot.libretro.com/docs/tech/licenses/).

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

!!! warning ""
	The King of Fighters '95 and Ultraman: Hikari no Kyojin Densetsu ROM Cartridges can be manually selected with the ['Cartridge' core option](https://buildbot.libretro.com/.docs/library/beetle_saturn/#core-options).

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
| Softpatching      | ✕         |

### Saves/States

The Beetle Saturn core's directory name is 'Mednafen Saturn'

Game data is saved/loaded to and from where save files are stored.

- .bcr (External cartridge backup save)
- .bkr (Internal save)
- .smpc (SMPC's emulated Real-Time Clock save)

Save states are saved/loaded to and from where state files are stored.

- .state (State)

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

!!! warning ""
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

- **System Region** (**Auto Detect**/Japan/North America/Europe/South Korea/Asia (NTSC)/Asia (PAL)/Brazil/Latin America): Choose which region the system is from.
- **Cartridge** (**Auto Detect**/None/Backup Memory/Extended RAM (1MB)/Extended RAM (4MB)/The King of Fighters '95/Ultraman: Hikari no Kyojin Densetsu): For information regarding The King of Fighters '95 ROM Cartridge and the Ultraman: Hikari no Kyojin Densetsu ROM Cartridge, please look at the [BIOS section](https://buildbot.libretro.com/.docs/library/beetle_saturn/#bios).
- **6Player Adaptor on Port 1** (**Off**/On): Enable [multitap](https://segaretro.org/Saturn_6_Player_Adaptor) on Saturn port 1.
- **6Player Adaptor on Port 2** (**Off**/On): Enable [multitap](https://segaretro.org/Saturn_6_Player_Adaptor) on Saturn port 2
- **3D Pad - Analog Deadzone** (0% to 30% in increments of 5%. **15% is default**): Configure the '3D Control Pad' Device Type's analog deadzone.
- **3D Pad - Trigger Deadzone** (0% to 30% in increments of 5%. **15% is default**): Configure the '3D Control Pad' Device Type's trigger deadzone.
- **Mouse - Sensitivity** (5% to 200% in increments of 5%. **100% is default**): Configure the 'Mouse' device type's sensitivity.
- **Gun - Crosshair** (**Cross**/Dot/Off): Choose the crosshair for the 'Stunner' and 'Virtua Gun' device types. Setting it to off disables the crosshair.

??? note "Gun - Crosshair - Cross"
	![crosshair_cross](images\Cores\beetle_saturn\crosshair_cross.png)
	
??? note "Gun - Crosshair - Dot"
	![crosshair_dot](images\Cores\beetle_saturn\crosshair_dot.png)

??? note "Gun - Crosshair - Off"
	![crosshair_off](images\Cores\beetle_saturn\crosshair_off.png)	

- **CD Image Cache (restart)** (**Off**/On): Loads the complete image in memory at startup.
- **Automatically set RTC on game load** (Off/**On**): Automatically set the SMPC's emulated Real-Time Clock to the host system's current time and date upon game load.
- **BIOS language** (**english**/german/french/spanish/italian/japanese): Self explanatory. Also affects language used in some games (e.g. the European release of "Panzer Dragoon").
- **Horizontal Overscan Mask** (0 to 60 in increments of 2. **0 is default**): Self-explanatory.
- **Initial scanline** (0 to 40 in increments of 1. **0 is default**): First displayed scanline in NTSC mode.
- **Last scanline** (210 to 239 in increments of 1. **239 is default**): First displayed scanline in PAL mode.
- **Initial scanline PAL** (0 to 60 in increments of 1. **16 is default**): Last displayed scanline in NTSC mode.
- **Last scanline PAL** (230 to 287 in increments of 1. **271 is default**): Last displayed scanline in PAL mode.
- **Enable Horizontal Blend(blur)** (**Off**/On): Self-explanatory.

??? note "Enable Horizontal Blend(blur) - Off"
	![blend_off](images\Cores\beetle_saturn\blend_off.png)
	
??? note "Enable Horizontal Blend(blur) - On"
	![blend_on](images\Cores\beetle_saturn\blend_on.png)

## Controllers

### Device types

The Beetle Saturn core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 12 device types

- [**Control Pad**](http://segaretro.org/Control_Pad_(Saturn)) - Joypad
- [**3D Control Pad**](http://segaretro.org/3D_Control_Pad) - Analog
- [**Arcade Racer**](http://segaretro.org/Arcade_Racer_Joystick) - Analog
- [**Mission Stick**](https://segaretro.org/Sega_Mission_Stick) - Analog
- [**Mouse**](http://segaretro.org/Shuttle_Mouse) - Mouse
- [**Stunner (US)**](http://segaretro.org/Virtua_Gun) - Lightgun
- [**Twin-Stick**](https://segaretro.org/Saturn_Twin-Stick) - Analog
- [**Virtua Gun (JP)**](https://segaretro.org/Virtua_Gun) - Lightgun

### Controllers graph

| Beetle Saturn                             | RetroPad                                                      | Control Pad  | 3D Control Pad | Arcade Racer              | Mission Stick              | Twin-Stick          |
|-------------------------------------------|---------------------------------------------------------------|--------------|----------------|---------------------------|----------------------------|---------------------|
| A Button                                  | ![](images/RetroPad/Retro_B_Round.png)                        | A Button     | A Button       | A Button                  | A Button                   |                     |
| X Button                                  | ![](images/RetroPad/Retro_Y_Round.png)                        | X Button     | X Button       | X Button                  | X Button                   |                     |
| Mode Switch                               | ![](images/RetroPad/Retro_Select.png)                         |              | Mode Switch    |                           |                            |                     |
| Start Button                              | ![](images/RetroPad/Retro_Start.png)                          | Start Button | Start Button   | Start Button              | Start Button               | Start Button        |
| D-Pad Up                                  | ![](images/RetroPad/Retro_Dpad_Up.png)                        | D-Pad Up     | D-Pad Up       |                           |                            |                     |
| D-Pad Down                                | ![](images/RetroPad/Retro_Dpad_Down.png)                      | D-Pad Down   | D-Pad Down     |                           |                            |                     |
| D-Pad Left                                | ![](images/RetroPad/Retro_Dpad_Left.png)                      | D-Pad Left   | D-Pad Left     |                           |                            |                     |
| D-Pad Right                               | ![](images/RetroPad/Retro_Dpad_Right.png)                     | D-Pad Right  | D-Pad Right    |                           |                            |                     |
| B Button                                  | ![](images/RetroPad/Retro_A_Round.png)                        | B Button     | B Button       | B Button                  | B Button                   |                     |
| Y Button                                  | ![](images/RetroPad/Retro_X_Round.png)                        | Y Button     | Y Button       | Y Button                  | Y Button                   |                     |
| Z Button                                  | ![](images/RetroPad/Retro_L1.png)                             | Z Button     | Z Button       | Z Button                  | Z Button                   | Left Stick Button   |
| C Button                                  | ![](images/RetroPad/Retro_R1.png)                             | C Button     | C Button       | C Button                  | C Button                   | Right Stick Button  |
| L Button                                  | ![](images/RetroPad/Retro_L2.png)                             | L Button     | L Button       | Left shift paddle (Up)    | L Button                   | Left Stick Trigger  |
| R Button                                  | ![](images/RetroPad/Retro_R2.png)                             | R Button     | R Button       | Right shift paddle (Down) | R Button                   | Right Stick Trigger |
|                                           | ![](images/RetroPad/Retro_R3.png)                             |              |                |                           | Throttle Latch             |                     |
| Analog X                                  | ![](images/RetroPad/Retro_Left_Stick.png)                     |              | Analog X       | Analog wheel              | Analog Stick X             | Left Stick X        |
| Analog Y                                  | ![](images/RetroPad/Retro_Left_Stick.png)                     |              | Analog Y       |                           | Analog Stick Y             | Left Stick Y        |
| Analog X (Right)                          | ![](images/RetroPad/Retro_Right_Stick.png)                    |              |                |                           |                            | Right Stick X       |
| Analog Y (Right)                          | ![](images/RetroPad/Retro_Right_Stick.png)                    |              |                |                           | Throttle                   | Right Stick Y       |

| RetroMouse                                                      | Mouse   |
|-----------------------------------------------------------------|---------|
| ![](images/RetroMouse/Retro_Mouse.png)                          | Pointer |
| ![](images/RetroMouse/Retro_Left.png)                           | A       |
| ![](images/RetroMouse/Retro_Right.png)                          | B       |
| ![](images/RetroMouse/Retro_Middle.png)                         | C       |
| Mouse Button 4                                                  | Start   |
| Mouse Button 5                                                  | Start   |

| Beetle Saturn        | Stunner | Virtua Gun |
|----------------------|---------|------------|
| Pointer              | Pointer | Pointer    |
| Gun Trigger          | Trigger | Trigger    |
| Gun Reload           | Reload  | Reload     |
| Gun Start            | Start   | Start      |

## External Links

- [Libretro Beetle Saturn Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_saturn_libretro.info)
- [Libretro Beetle Saturn Github Repository](https://github.com/libretro/beetle-saturn-libretro)
- [Report Libretro Beetle Saturn Core Issues Here](https://github.com/libretro/beetle-saturn-libretro/issues)
- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)