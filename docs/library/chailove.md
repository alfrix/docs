# ChaiLove

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/chailove.md). Changes are proposed using "Pull Requests."

There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)

You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).

## Background

[ChaiLove](https://github.com/RobLoach/ChaiLove) is a framework for making 2D games with [ChaiScript](http://chaiscript.com/). ChaiLove games can be played with LibRetro/RetroArch through the ChaiLove core.

### Why use this core?

Awaiting description.

### How to get and install the ChaiLove core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'ChaiLove'.

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'ChaiLove'.

The content should now start running!

##### Extra example

As an extra example showcasing loading content with Chailove core, we will load the Floppy Bird game hosted on RetroArch's Content Downloader.

1. First, you need to obtain Floppy Bird's data files. You can do this by going to RetroArch's main menu screen. From there, select 'Content Downloader'.

2. Select 'ChaiLove', then select 'Floppy Bird.chailove'. This should download and extract this file to RetroArch's Downloads directory.

3. Go back to RetroArch's main menu screen. Select 'Load Content', then 'Downloads'.

4. Select 'Floppy Bird.chailove'

5. If you are asked which core to select, choose 'ChaiLove'.

The content should now start running!

### Authors

- Rob Loach

## See also

### Custom engine

- [Lua Engine (Lutro)](https://docs.libretro.com/library/lutro/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

- [MIT](https://github.com/RobLoach/ChaiLove/blob/master/LICENSE.md)

## Extensions

Content that can be loaded by the ChaiLove core have the following file extensions:

- .chai
- .chailove

## Databases

RetroArch database(s) that are associated with the ChaiLove core:

- [ChaiLove](https://github.com/libretro/libretro-database/blob/master/rdb/ChaiLove.rdb)

## Features

RetroArch-level settings or features that the ChaiLove core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✕         |
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
| Softpatching      | ✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The ChaiLove core's directory name is 'ChaiLove'

The ChaiLove core saves/loads to/from these directories.

**RetroArch's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The ChaiLove core's internal FPS is 60
- The ChaiLove core's internal sample rate is 44100 Hz
- The ChaiLove core's core provided aspect ratio is (Ratio)

## Core options

The ChaiLove core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

- **Alpha Blending** (Off/**On**) 

<center> Enable or disable alpha blending (transparency). </center>

??? note "Alpha Blending - On"
	![](images\Cores\chailove\alpha_on.png)
	
??? note "Alpha Blending - Off"
	![](images\Cores\chailove\alpha_off.png)	

- **High Quality** (Off/**On**)

<center> Enable or disable extra visual features. </center>

??? note "High Quality - On"
	![](images\Cores\chailove\quality_on.png)
	
??? note "High Quality - Off"
	![](images\Cores\chailove\quality_off.png)	

## Controllers

### Device types

The ChaiLove core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 5 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There's no reason to switch to this.

### Controller tables

#### Joypad and analog device type table

!!! attention
	**What the buttons do are game specific.**

| Users 1 - 5 Input descriptors | RetroPad Inputs                              |
|-------------------------------|----------------------------------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       |
| Y                             | ![](images/RetroPad/Retro_Y_Round.png)       |           
| Select                        | ![](images/RetroPad/Retro_Select.png)        |
| Start                         | ![](images/RetroPad/Retro_Start.png)         |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       |
| X                             | ![](images/RetroPad/Retro_X_Round.png)       |
| L                             | ![](images/RetroPad/Retro_L1.png)            |
| R                             | ![](images/RetroPad/Retro_R1.png)            |

## External Links

- [Libretro ChaiLove Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/chailove_libretro.info)
- [Official/Libretro ChaiLove Github Repository](https://github.com/RobLoach/ChaiLove)
- [Report Libretro ChaiLove Core Issues Here](https://github.com/RobLoach/ChaiLove/issues)
- [ChaiLove API Documentation Website](https://robloach.github.io/ChaiLove/)
- [ChaiScript Website](http://chaiscript.com/)