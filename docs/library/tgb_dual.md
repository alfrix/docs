# Game Boy / Game Boy Color (TGB Dual)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/tgb_dual.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

TGB Dual is an open source (GPLv2) GB/GBC emulator with game link cable support.

### Why use this core?

Awaiting description.

### How to get and install the TGB Dual core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Game Boy / Game Boy Color (TGB Dual)'.

<center> ![](images\Cores\tgb_dual\tgb_dual.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\tgb_dual\sheepitup.png) </center>

- If you are asked which core to select, choose 'Game Boy / Game Boy Color (TGB Dual)'.

The content should now start running!

### Authors

- GIGO
- Hii

## See also

### GB/GBC

- [Game Boy / Game Boy Color (Emux GB)](https://docs.libretro.com/library/emux_gb/)
- [Game Boy / Game Boy Color (Gambatte)](https://docs.libretro.com/library/gambatte/)
- [Game Boy / Game Boy Color (SameBoy)](https://docs.libretro.com/library/sameboy/)
- [Game Boy / Game Boy Color (Gearboy)](https://docs.libretro.com/library/gearboy/)
- [Game Boy Advance (mGBA)](https://docs.libretro.com/library/mgba/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The TGB Dual core is licensed under

- [GPLv2](https://github.com/libretro/tgbdual-libretro/blob/master/docs/COPYING-2.0.txt)

## Extensions

Content that can be loaded by the TGB Dual core have the following file extensions:

- .gb
- .gbc
- .sgb

## Databases

RetroArch database(s) that are associated with the TGB Dual core:

- [Nintendo - Game Boy](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy.rdb)
- [Nintendo - Game Boy Color](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Color.rdb)

## Features

RetroArch-level settings or features that the TGB Dual core respects.

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
| Softpatching      | ✔         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The TGB Dual core's directory name is 'TGB Dual'

The TGB Dual core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge battery save)
- 'content-name'.rtc (Real time clock save)

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The TGB Dual core's internal FPS is 59.72
- The TGB Dual core's internal sample rate is 44100 Hz
- The TGB Dual core's core provided aspect ratio is (Ratio)

### Usage

Awaiting description.

## Core options

The TGB Dual core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **GB Link Enable (Restart)** (**Off**/On) (restart)

<center> Emulates two Game Boy units side by side for multiplayer support. </center>

??? note "*GB Link Enable - Enabled*"
    ![](images\Cores\tgb_dual\link.png)

- **Screen placement** (**horizontal**/vertical)

<center> Switches the screen layout for multiplayer support. </center>

??? note "*Horizontal*"
    ![](images\Cores\tgb_dual\horiz.png)

??? note "*Vertical*"
    ![](images\Cores\tgb_dual\vert.png)

- **Switch player screens** (**normal**/switched)

<center> Switches the player screens for multiplayer support. </center>

- **Show player screens** (**both players**/player 1 only/player 2 only)

<center> Displays the selected player screens for multiplayer support. </center>

## Controllers

### Device types

The TGB Dual core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 2 device types

- None - Input isn't disabled.
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There is no reason to switch to this.

### Controller tables

#### Joypad and analog device type table

| User 1 - 2 Input descriptors  | RetroPad Inputs                              |
|-------------------------------|----------------------------------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       |
| Select                        | ![](images/RetroPad/Retro_Select.png)        |
| Start                         | ![](images/RetroPad/Retro_Start.png)         |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       |
| Prev Audio Mode               | ![](images/RetroPad/Retro_L1.png)            |
| Next Audio Mode               | ![](images/RetroPad/Retro_R1.png)            |

## Compatibility

Awaiting description.

## External Links

- [Libretro TGB Dual Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/tgbdual_libretro.info)
- [Libretro TGB Dual Github Repository](https://github.com/libretro/tgbdual-libretro)
- [Report Libretro TGB Dual Core Issues Here](https://github.com/libretro/tgbdual-libretro/issues)
- [Official TGB Dual Website](http://gigo.retrogames.com/download.html#tgb-dual)
- [Official TGB Dual SDL port Website](http://shinh.skr.jp/tgbdualsdl/)