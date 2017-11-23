# Sega Saturn (Beetle Saturn)

## Background

Port of standalone Mednafen Saturn to libretro

### Why use this core?

Awaiting description.

### Authors

- Mednafen Team

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/beetle_saturn.md). Changes are proposed using "Pull Requests."

## See also

- [Sega Saturn (Yabause)](https://buildbot.libretro.com/docs/library/Yabause/)

## License

- GPLv2

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

|   Filename       |    Description                                                             |              md5sum              |
|:----------------:|:--------------------------------------------------------------------------:|:--------------------------------:|
| sega_101.bin     | Saturn JP BIOS - Required                                                  | 85ec9ca47d8f6807718151cbcca8b964 |
| mpr-17933.bin    | Saturn US/EU BIOS - Required                                               | 3240872c70984b6cbfda1586cab68dbe |
| mpr-18811-mx.ic1 | The King of Fighters '95 ROM Cartridge - Required for this game            | 255113ba943c92a54facd25a10fd780c |
| mpr-19367-mx.ic1 | Ultraman: Hikari no Kyojin Densetsu ROM Cartridge - Required for this game | 1cd19988d1d72a3e7caa0b73234c96b4 |

**The King of Fighters '95 ROM Cartridge or the Ultraman: Hikari no Kyojin Densetsu ROM Cartridge will only be used when the ['Cartridge' core option](https://buildbot.libretro.com/docs/library/beetle_saturn/#options) is set to use one of them.**

### Core Option

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
| Softpatching      | -         |

The Beetle Saturn core's directory name is 'Mednafen Saturn'

- Game data is saved/loaded to and from where save files are stored.
- Save states are saved/loaded to and from where state files are stored.

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

The Beetle Saturn core has the following options that can be tweaked from the core options menu. The default setting is bolded.

- **System Region** (**Auto Detect**/Japan/North America/Europe/South Korea/Asia (NTSC)/Asia (PAL)/Brazil/Latin America): Choose which region the system is from.
- **Cartridge** (**Auto Detect**/None/Backup Memory/Extended RAM (1MB)/Extended RAM (4MB)/The King of Fighters '95/Ultraman: Hikari no Kyojin Densetsu): For information regarding The King of Fighters '95 ROM Cartridge and the Ultraman: Hikari no Kyojin Densetsu ROM Cartridge, please look at the [BIOS section](https://buildbot.libretro.com/docs/library/beetle_saturn/#bios) 
- **3D Pad - Analog Deadzone** (0% to 30% in increments of 5%. **15% is default**): Configure the '3D Control Pad' Device Type's analog deadzone.
- **3D Pad - Trigger Deadzone** (0% to 30% in increments of 5%. **15% is default**): Configure the '3D Control Pad' Device Type's trigger deadzone.
- **Mouse - Sensitivity** (5% to 200% in increments of 5%. **100% is default**): Configure the 'Mouse' Device Type's sensitivity.
- **Virtua Gun - Crosshair** (**Cross**/Dot/Off): Choose the crosshair for the 'Virtua Gun / Stunner' Device Type. Setting it to off disables the crosshair.

??? note "Virtua Gun - Crosshair - Cross"
	![crosshair_cross](images\Cores\beetle_saturn\crosshair_cross.png)
	
??? note "Virtua Gun - Crosshair - Dot"
	![crosshair_dot](images\Cores\beetle_saturn\crosshair_dot.png)

??? note "Virtua Gun - Crosshair - Off"
	![crosshair_off](images\Cores\beetle_saturn\crosshair_off.png)	

- **Virtua Gun - Trigger** (**Left Mouse Button**/Right Mouse Button): Select whether the left or right mouse button is used as the trigger for the 'Virtua Gun / Stunner' Device Type. Look below at the [Controllers graph](https://buildbot.libretro.com/docs/library/beetle_saturn/#controllers-graph) section for more information.
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

The Beetle Saturn core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):

### User 1 - 2 Device Types

- [**Control Pad**](http://segaretro.org/Control_Pad_(Saturn)) - Joypad
- [**3D Control Pad**](http://segaretro.org/3D_Control_Pad) - Joypad - To avoid compatibility issues, the 3D Pad has a switch to swap between "Digital" and "Analogue" modes. Switching to "Digital" mode disables all analog settings, essentially turning the controller back into a standard Control Pad.
- [**Arcade Racer**](http://segaretro.org/Arcade_Racer_Joystick) - Joypad
- [**Mouse**](http://segaretro.org/Shuttle_Mouse) - Mouse
- [**Virtua Gun / Stunner**](http://segaretro.org/Virtua_Gun) - Lightgun

### User 3 - 16 Device Types

- **RetroPad** - Joypad

### Controllers graph

| Beetle Saturn | RetroPad                                                     | Control Pad  | 3D Control Pad | Arcade Racer              |
|--------------|---------------------------------------------------------------|--------------|----------------|---------------------------|
| A Button     | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)              | A Button     | A Button       | A Button                  |
| X Button     | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)              | X Button     | X Button       | X Button                  |
| Mode Switch  | ![RetroPad_Select](images/RetroPad/Retro_Select.png)          |              | Mode Switch    |                           |
| Start Button | ![RetroPad_Start](images/RetroPad/Retro_Start.png)            | Start Button | Start Button   | Start                     |
| D-Pad Up     | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)           | D-Pad Up     | D-Pad Up       |                           |
| D-Pad Down   | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)         | D-Pad Down   | D-Pad Down     |                           |
| D-Pad Left   | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)         | D-Pad Left   | D-Pad Left     |                           |
| D-Pad Right  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)        | D-Pad Right  | D-Pad Right    |                           |
| B Button     | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)              | B Button     | B Button       | B Button                  |
| Y Button     | ![RetroPad_X](images/RetroPad/Retro_X_Round.png)              | Y Button     | Y Button       | Y Button                  |
| Z Button     | ![RetroPad_L1](images/RetroPad/Retro_L1.png)                  | Z Button     | Z Button       | Z Button                  |
| C Button     | ![RetroPad_R1](images/RetroPad/Retro_R1.png)                  | C Button     | C Button       | C Button                  |
| L Button     | ![RetroPad_L2](images/RetroPad/Retro_L2.png)                  | L Button     | L Button       | Left shift paddle (Up)    |
| R Button     | ![RetroPad_R2](images/RetroPad/Retro_R2.png)                  | R Button     | R Button       | Right shift paddle (Down) |
| Analog X     | ![RetroPad_Left_Stick](images/RetroPad/Retro_Left_Stick.png)  |              | Analog X       | Analog wheel              |
| Analog Y     | ![RetroPad_Left_Stick](images/RetroPad/Retro_Left_Stick.png)  |              | Analog Y       |                           |

| RetroMouse                                                      | Mouse   | Virtua Gun / Stunner |
|-----------------------------------------------------------------|---------|----------------------|
| ![Retro_Mouse](images/RetroMouse/Retro_Mouse.png)               | Pointer | Pointer              |
| ![Retro_Left](images/RetroMouse/Retro_Left.png)                 | A       | Trigger†             |
| ![Retro_Right](images/RetroMouse/Retro_Right.png)               | B       | Start†               |
| ![Retro_Middle](images/RetroMouse/Retro_Middle.png)             | C       |                      |
| Mouse Button 4                                                  | Start   |                      |
| Mouse Button 5                                                  | Start   |                      |

† These inputs can be modified with the ['Virtua Gun - Trigger' core option](https://buildbot.libretro.com/docs/library/beetle_saturn/#core-options).

**If the 'Virtua Gun - Trigger' core option is set to Left Mouse Button, then**

- Left click = Virtua Gun / Stunner 'Trigger'
- Right click = Virtua Gun / Stunner 'Start'

**If the 'Virtua Gun - Trigger' core option is set to  Right Mouse Button, then**

- Left click = Virtua Gun / Stunner 'Start'
- Right click = Virtua Gun / Stunner 'Trigger'

## External Links

- [Libretro Beetle Saturn Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mednafen_saturn_libretro.info)
- [Libretro Beetle Saturn Github Repository](https://github.com/libretro/beetle-saturn-libretro)
- [Report Libretro Beetle Saturn Core Issues Here](https://github.com/libretro/beetle-saturn-libretro/issues)
- [Official Mednafen Website](https://mednafen.github.io/)
- [Official Mednafen Downloads](https://mednafen.github.io/releases/)