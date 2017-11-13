# ChaiLove

## Background

ChaiLove is a framework for making 2D games with [ChaiScript](http://chaiscript.com/). ChaiLove games can be played with LibRetro/RetroArch through the ChaiLove core.

### Usage

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'ChaiLove'.

4. After this has finished downloading, you will now need a ChaiLove game. We will be using Floppy Bird as an example. You can obtain Floppy Bird by going back to the previous menu screen. From there, select 'Content Downloader'.

5. Select 'ChaiLove', then select 'Floppy Bird.chailove'. This should download and extract this file to RetroArch's Downloads directory.

#### How to play

1. Go back to RetroArch's main menu screen. Select 'Load Content', then 'Downloads'.

2. Select 'Floppy Bird.chailove'

3. If you are asked which core to select, choose 'ChaiLove'.

The game should now start running!

### Author(s):

Rob Loach

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/chailove.md). Changes are proposed using "Pull Requests."

## License

MIT

## Extensions

*Content that can be loaded by the ChaiLove core have the following file extensions.*

chai|chailove|chaigame

## Database(s)

*RetroArch database(s) that are associated with the ChaiLove core*

* ChaiLove

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✕         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| RetroAchievements | ✕         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controllers       | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |

The ChaiLove core's directory name is 'ChaiLove'

Save states are saved/loaded to and from where state files are stored. 

## Core options

*The ChaiLove core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.*

- **Alpha Blending** (Off/**On**): Enable or disable alpha blending (transparency).

??? note "Alpha Blending - On"
	![alpha_blending_on](images\Cores\chailove\alpha_blending_on.png)
	
??? note "Alpha Blending - Off"
	![alpha_blending_off](images\Cores\chailove\alpha_blending_off.png)	

- **High Quality** (Off/**On**): Enable or disable extra visual features.

??? note "High Quality - On"
	![high_quality_on](images\Cores\chailove\high_quality_on.png)
	
??? note "High Quality - Off"
	![high_quality_off](images\Cores\chailove\high_quality_off.png)	

## Controllers

*The ChaiLove core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):*

### User 1 - 16 Device Type(s)

* **RetroPad** - Joypad with analog

* RetroPad w/Analog - **There is no reason to switch to this**

### Controllers graph

| ChaiLove    | RetroPad                                                       |
|-------------|----------------------------------------------------------------|
| B           | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               |
| Y           | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)               |
| Select      | ![RetroPad_Select](images/RetroPad/Retro_Select.png)           |
| Start       | ![RetroPad_Start](images/RetroPad/Retro_Start.png)             |
| D-Pad Up    | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            |
| D-Pad Down  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          |
| D-Pad Left  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          |
| D-Pad Right | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         |
| A           | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               |
| X           | ![RetroPad_X](images/RetroPad/Retro_X_Round.png)               |
| L           | ![RetroPad_L1](images/RetroPad/Retro_L1.png)                   |
| R           | ![RetroPad_R1](images/RetroPad/Retro_R1.png)                   |

## External Links

* [Official/Libretro Repository](https://github.com/RobLoach/ChaiLove)
* [Report Core Issues Here](https://github.com/RobLoach/ChaiLove/issues)