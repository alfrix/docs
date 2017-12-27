# Game Boy Advance (mGBA)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/mgba.md). Changes are proposed using "Pull Requests."

## Background

mGBA is an emulator for running Game Boy Advance games. It aims to be faster and more accurate than many existing Game Boy Advance emulators, as well as adding features that other emulators lack.

### Why use this core?

Awaiting description.

### How to get and install the mGBA core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Game Boy Advance (mGBA)'.

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'Game Boy Advance (mGBA)'.

The content should now start running!

### Authors

- endrift

## See also

### GBA

- [Game Boy Advance (Beetle GBA)](https://docs.libretro.com/library/beetle_gba/)
- [Game Boy Advance (gpSP)](https://docs.libretro.com/library/gpsp/)
- [Game Boy Advance (Meteor)](https://docs.libretro.com/library/meteor/)
- [Game Boy Advance (VBA Next)](https://docs.libretro.com/library/vba_next/)
- [Game Boy Advance (VBA-M)](https://docs.libretro.com/library/vbam/)

### GB/GBC

- [Game Boy / Game Boy Color (Emux)](https://docs.libretro.com/library/emux_gb/)
- [Game Boy / Game Boy Color (Gambatte)](https://docs.libretro.com/library/gambatte/)
- [Game Boy / Game Boy Color (SameBoy)](https://docs.libretro.com/library/sameboy/)
- [Game Boy / Game Boy Color (TGB Dual)](https://docs.libretro.com/library/tgb_dual/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

- [MPLv2.0](https://github.com/libretro/mgba/blob/master/LICENSE)

## Extensions

Content that can be loaded by the mGBA core have the following file extensions:

- .gb
- .gbc
- .gba

## Databases

RetroArch database(s) that are associated with the mGBA core:

- [Nintendo - Game Boy](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy.rdb)
- [Nintendo - Game Boy Color](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Color.rdb)
- [Nintendo - Game Boy Advance](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Advance.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

|   Filename    |    Description                  |              md5sum              |
|:-------------:|:-------------------------------:|:--------------------------------:|
| gba_bios.bin  |Game Boy Advance BIOS - Optional | a860e8c0b6d573d191e4ec7db1b1e4f6 |

!!! warning
	In order for the Game Boy Advance BIOS to be used, the 'Use BIOS file if found' core option must be set to On.
	
## Features

RetroArch features that the mGBA core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔ (not link-cable emulation) |
| Core Options      | ✔         |
| RetroAchievements | ✔ (GBA only) |
| RetroArch Cheats  | ✔         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | ✕         |
| Rumble            | ✔         |
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

The mGBA core's directory name is 'mGBA'

The mGBA loads from and saves to to these directories.

RetroArch's Save directory

- 'content-name'.srm (Cartridge battery save)

RetroArch's State directory

- 'content-name'.state# (State)

### Geometry and timing

The mGBA core's internal FPS is (FPS).

The mGBA core's internal sample rate is 32768 Hz.

The mGBA core's core provided aspect ratio is (Ratio).

### Rumble

Rumble only works in the mGBA core when

- The content being ran has rumble support. (e.g. Cartridges with a Rumble Pak)
- The joypad input driver being used has rumble support. (e.g. Xinput)
- The joypad device being used has rumble support. (e.g. Xbox 360 Controller)

## Core options

The mGBA core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Solar sensor level** (0 to 10 in increments of 1. **0 is default.**)

<center> Can be used for games that employed the use of a solar sensor on their cartridges. </center>

- **Allow opposing directional input** (**Off**/On)

<center> Awaiting description. </center>

- **Use BIOS file if found** (Off/**On**)

<center> Uses a Game Boy Advance BIOS present in RetroArch's system directory. Please look at the [BIOS section](https://buildbot.libretro.com/.docs/library/mgba/index.html#bios) for more information. </center>

- **Skip BIOS intro** (**Off**/On)

<center> Skips the BIOS intro when a Game Boy Advance BIOS present in RetroArch's system directory is used. The 'Use BIOS file if found' core option must be set to On for proper operation. </center>

<center>

??? note "Skip BIOS intro - Off"
    ![bios](images\Cores\mgba\bios.png)
	
</center>

- **Idle loop removal** (**Remove Known**/Detect and Remove/Don't Remove)

<center> Awaiting description. </center>

## Controllers

### Device types

The mGBA core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There is no reason to switch to this.

### Controller tables

#### Joypad and analog device type table

| User 1 input descriptors      | RetroPad Inputs                              | RetroPad              |
|-------------------------------|----------------------------------------------|-----------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                     |
| Turbo B                       | ![](images/RetroPad/Retro_Y_Round.png)       | Turbo B               |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select                |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start                 |
| Up                            | ![](images/RetroPad/Retro_Dpad_Up.png)       | Up                    |
| Down                          | ![](images/RetroPad/Retro_Dpad_Down.png)     | Down                  |
| Left                          | ![](images/RetroPad/Retro_Dpad_Left.png)     | Left                  |
| Right                         | ![](images/RetroPad/Retro_Dpad_Right.png)    | Right                 |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | A                     |
| Turbo A                       | ![](images/RetroPad/Retro_X_Round.png)       | Turbo A               |
| L                             | ![](images/RetroPad/Retro_L1.png)            | L                     |
| R                             | ![](images/RetroPad/Retro_R1.png)            | R                     |
| Turbo L                       | ![](images/RetroPad/Retro_L2.png)            | Turbo L               |
| Turbo R                       | ![](images/RetroPad/Retro_R2.png)            | Turbo R               |
| Darken Solar Sensor           | ![](images/RetroPad/Retro_L3.png)            | Darken Solar Sensor   |
| Brighten Solar Sensor         | ![](images/RetroPad/Retro_R3.png)            | Brighten Solar Sensor |

## Compatibility

Awaiting description.

## External Links

- [Libretro mGBA Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mgba_libretro.info)
- [Libretro mGBA Github Repository](https://github.com/libretro/mgba)
- [Report Libretro mGBA Core Issues Here](https://github.com/libretro/mgba/issues)
- [Official mGBA Website](https://mgba.io/)
- [Official mGBA Github Repository](https://github.com/mgba-emu/mgba)
