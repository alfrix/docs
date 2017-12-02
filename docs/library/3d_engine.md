# 3D Engine

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/3d_engine.md). Changes are proposed using "Pull Requests."

## Background

A tech demo for libretro GL with additional features (camera/location/etc).

### How to get and install the 3D Engine core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select '3D Engine'.

After this has finished downloading, the core should now be ready for use!

### Authors

- Team Libretro

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://buildbot.libretro.com/docs/tech/licenses/).

- [GPLv3](https://github.com/libretro/libretro-3dengine/blob/master/license)

## Extensions

Content that can be loaded by the 3D Engine core have the following file extensions:

- .png
- .jpg
- .mtl
- .obj

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
| Remapping         | ✕         |
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✔         |
| Camera            | ✔         |
| Location          | ✔         |
| Subsystem         | ✕         |
| Softpatching      | ✕         |

### Saves/States

The 3D Engine core's directory name is 'Libretro 3DEngine'

## Core options

The 3D Engine core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.

- **Internal resolution** (**320x240**/360x480/480x272/512x384/512x512/640x240/640x448/640x480/720x576/800x600/960x720/1024x768/1024x1024/1280x720/1280x960/1600x1200/1920x1080/1920x1440/1920x1600/2048x1152/2048x1536/2048x2048/320x240): Configure the resolution.
- **Cube size** (**0**/1/2/4/8/16/32/64/128): Awaiting description.
- **Cube stride** (2.0 to 8.0 in increments of 1.0. **2.0 is default**): Awaiting description.
- **Camera enable** (**Off**/On): Awaiting description.
- **Camera FB Type** (**texture/**/raw framebuffer): Awaiting description.
- **Sensor enable** (**Off**/On): Awaiting description.
- **Location enable** (**Off**/On): Awaiting description.
- **Location camera control** (**Off**/On): Awaiting description.
- **Discard hack enable** (**Off**/On): Awaiting description.
- **Location position OSD** (**Off**/On): Awaiting description.

## Controllers

The 3D Engine core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 device types

- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - **There is no reason to switch to this.**

### Controllers graph

| 3D Engine                                | RetroPad                                                       |
|------------------------------------------|----------------------------------------------------------------|
| Jump/Zoom-in                             | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               |
| Move forwards                            | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            |
| Move backwards                           | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          |
| Turn left                                | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          |
| Turn right                               | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         |
| Zoom-out                                 | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               |
| Move Left                                | ![RetroPad_L1](images/RetroPad/Retro_L1.png)                   |
| Move Right                               | ![RetroPad_R1](images/RetroPad/Retro_R1.png)                   |
| Adjust lighting                          | ![RetroPad_L2](images/RetroPad/Retro_L2.png)                   |
| Adjust lighting                          | ![RetroPad_R2](images/RetroPad/Retro_R2.png)                   |
| Adjust lighting                          | ![RetroPad_R3](images/RetroPad/Retro_R3.png)                   |
| Move right or left/Rotate model          | ![RetroPad_Left_Stick](images/RetroPad/Retro_Left_Stick.png)   |
| Move forwards and backwards/Rotate model | ![RetroPad_Left_Stick](images/RetroPad/Retro_Left_Stick.png)   |
| Look right and left                      | ![RetroPad_Right_Stick](images/RetroPad/Retro_Right_Stick.png) |
| Look up and down/Zoom-in or Zoom-out     | ![RetroPad_Right_Stick](images/RetroPad/Retro_Right_Stick.png) |

## External Links

- [Libretro 3D Engine Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/3dengine_libretro.info)
- [Libretro 3D Engine Github Repository](https://github.com/libretro/libretro-3dengine)
- [Report Libretro 3D Engine Core Issues Here](https://github.com/libretro/libretro-3dengine/issues)