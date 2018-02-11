# Lua Engine (Lutro)

## Background

Lutro is an experimental lua game framework that follows the [LÖVE API](https://love2d.org/wiki/Main_Page). Lutro games can be played with LibRetro/RetroArch through the Lutro core. 

### Usage

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Lua Engine (Lutro)'.

4. After this has finished downloading, you will now need a Lutro game. We will be using Pong as an example. You can obtain Pong by going back to the previous menu screen. From there, select 'Content Downloader'.

5. Select 'Lutro', then select 'Pong.lutro'. This should download and extract this file to RetroArch's Downloads directory.

#### How to play

1. Go back to RetroArch's main menu screen. Select 'Load Content', then 'Downloads'.

2. Select 'Pong.lutro'

3. If you are asked which core to select, choose 'Lutro'.

The game should now start running!

### Author(s):

Higor Euripedes/Jean-Andre Santoni

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/lutro.md). Changes are proposed using "Pull Requests."

## See also

[ChaiLove](https://docs.libretro.com/library/chailove/)

## License

MIT

## Extensions

*Content that can be loaded by the Lutro core have the following file extensions.*

lutro|lua

## Database(s)

*RetroArch database(s) that are associated with the Lutro core*

* Lutro

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✕         |
| States            | ✕         |
| Rewind            | ✕         |
| Netplay           | ✕         |
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

The Lutro core's directory name is 'lutro'

## Controllers

*The Lutro core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):*

### User 1 - 16 Device Type(s)

* **RetroPad** - Joypad 

* RetroPad w/Analog - Joypad - **There is no reason to switch to this.**

### Controllers graph

**What the buttons do are game specific.**

| Lutro     | RetroPad                                                       |
|-----------|----------------------------------------------------------------|
| B         | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               |
| Y         | ![RetroPad_Y](images/RetroPad/Retro_Y_Round.png)               |
| Select    | ![RetroPad_Select](images/RetroPad/Retro_Select.png)           |
| Start     | ![RetroPad_Start](images/RetroPad/Retro_Start.png)             |
| Up        | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            |
| Down      | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          |
| Left      | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          |
| Right     | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         |
| A         | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               |
| X         | ![RetroPad_X](images/RetroPad/Retro_X_Round.png)               |

## External Links

* [Official/Libretro Repository](https://github.com/libretro/libretro-lutro)
* [Report Core Issues Here](https://github.com/libretro/libretro-meta)