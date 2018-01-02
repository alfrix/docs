# Handheld Electronic (GW)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/gw.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

A libretro core for Game & Watch simulators.

It runs simulators converted from source code for the games available at [MADrigal](http://www.madrigaldesign.it/sim/).

### Why use this core?

Awaiting description.

### How to get and install the GW core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Handheld Electronic (GW)'.

<center> ![](images\Cores\gw\gw.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'Handheld Electronic (GW)'.

The content should now start running!

##### Extra example

As an extra example showcasing loading content with GW core, we will load the Donkey Kong (Coleco) game hosted on RetroArch's Content Downloader.

1. First, you need to obtain Donkey Kong (Coleco)'s data files. You can do this by going to RetroArch's main menu screen. From there, select 'Content Downloader'.

2. Select 'Handheld Electronic Game', then select 'Donkey Kong (Coleco).zip'. This should download and extract this file to RetroArch's Downloads directory.

3. Go back to RetroArch's main menu screen. Select 'Load Content', then 'Downloads'.

4. Select 'Donkey Kong (Coleco).mgw'

5. If you are asked which core to select, choose 'Handheld Electronic (GW)'.

The content should now start running!

### Authors

- Andre Leiradella

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The GW core is licensed under

- [zlib](https://github.com/libretro/gw-libretro/blob/master/LICENSE)

## Extensions

Content that can be loaded by the GW core have the following file extensions:

- .mgw

## Databases

RetroArch database(s) that are associated with the GW core:

- [Handheld Electronic Game](https://github.com/libretro/libretro-database/blob/master/rdb/Handheld%20Electronic%20Game.rdb)

## Features

RetroArch-level settings or features that the GW core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✕         |
| Screenshots       | ✔         |
| Saves             | ✕         |
| States            | ✕         |
| Rewind            | ✕         |
| Netplay           | ✕         |
| Core Options      | ✕         |
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
| Crop Overscan     | ✕         |

### Directories

The GW core's directory name is 'Game & Watch'

### Geometry and timing

- The GW core's internal FPS is 60
- The GW core's internal sample rate is 44100 Hz
- The GW core's core provided aspect ratio is (Ratio)

## Controllers

### Device types

The GW core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 2 device types

- None - Input disabled.
- **Controller** - Joypad

### Controller tables

#### Joypad and analog device type table

| User 1 Remap descriptors      | RetroPad Inputs                              | Controller         |
|-------------------------------|----------------------------------------------|--------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | †                  |
| Y                             | ![](images/RetroPad/Retro_Y_Round.png)       | †                  |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Menu               |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Select             |
| Up                            | ![](images/RetroPad/Retro_Dpad_Up.png)       | †                  |
| Down                          | ![](images/RetroPad/Retro_Dpad_Down.png)     | †                  |
| Left                          | ![](images/RetroPad/Retro_Dpad_Left.png)     | †                  |
| Right                         | ![](images/RetroPad/Retro_Dpad_Right.png)    | †                  |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | †                  |
| X                             | ![](images/RetroPad/Retro_X_Round.png)       | †                  |
| L1                            | ![](images/RetroPad/Retro_L1.png)            | †                  |
| R1                            | ![](images/RetroPad/Retro_R1.png)            | †                  |
| L2                            | ![](images/RetroPad/Retro_L2.png)            | †                  |
| R2                            | ![](images/RetroPad/Retro_R2.png)            | †                  |
| L3                            | ![](images/RetroPad/Retro_L3.png)            | †                  |
| R3                            | ![](images/RetroPad/Retro_R3.png)            | †                  |

† What these inputs do are game specific.

!!! attention
	Without having anything selected, you can use the Select input to see a Controller overlay to see what the game specific inputs are.

## Compatibility

Awaiting description.

## External Links

- [Libretro GW Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/gw_libretro.info)
- [Libretro GW Github Repository](https://github.com/libretro/gw-libretro)
- [Report Libretro GW Core Issues Here](https://github.com/libretro/gw-libretro/issues)
- [MADrigal Website](http://www.madrigaldesign.it/sim/)