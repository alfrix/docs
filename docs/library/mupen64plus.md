# Nintendo 64 (Mupen64Plus)

## Contribute to this documentation

**DOCUMENTATION IS A WORK IN PROGRESS**

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/mupen64plus.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Mupen64Plus uses GLideN64

### Why use this core?

Awaiting description.

### How to get and install the Mupen64Plus core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'Nintendo 64 (Mupen64Plus)'.

<center> ![](images\Cores\updater\mupen64plus.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):
- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

- If you are asked which core to select, choose 'Nintendo 64 (Mupen64Plus)'.

The content should now start running!

### Authors

- Hacktarux
- Mupen64Plus Team


## See also

### N64

- [Nintendo 64 (ParaLLEl N64)](https://docs.libretro.com/library/parallel/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Mupen64Plus core is licensed under

- [GPLv3](https://github.com/libretro/mupen64plus-libretro/blob/master/LICENSE)

## Extensions

Content that can be loaded by the Mupen64Plus core have the following file extensions:

- .n64
- .v64
- .z64
- .bin
- .u1
- .ndd

## Databases

RetroArch database(s) that are associated with the Mupen64Plus core:

- [Nintendo - Nintendo 64](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Nintendo%2064.rdb)
- [Nintendo - Nintendo 64DD](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Nintendo%2064DD.rdb)

## Features

RetroArch-level settings or features that the Mupen64Plus core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| Core Options      | ✔         |
| RetroAchievements | ✔         |
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
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | ✕         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✕         |

### Directories

The Mupen64Plus core's directory name is 'Mupen64Plus OpenGL'

The Mupen64Plus core saves/loads to/from these directories.

**RetroArch's Save directory**

- 'content-name'.srm (Cartridge backup save)

**RetroArch's State directory**

- 'content-name'.state# (State)

**RetroArch's System directory**

```
- Mupen64plus/
			- mupen64plus.ini
			- shaders/
```

### Geometry and timing

- The Mupen64Plus core's internal FPS is (FPS)
- The Mupen64Plus core's internal sample rate is 44100 Hz
- The Mupen64Plus core's core provided aspect ratio is (Ratio)

###  Hi res Textures

Awaiting description.

## Core options

The Mupen64Plus core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded. 

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

 - **CPU Core** (**dynamic_recompiler**/cached_interpreter/pure_interpreter)

	Choose which kind of CPU emulation is going to be used.
	
	**Dynamic recompilier is not available on all platforms.**
	
- **RSP Mode** (**HLE**/LLE)

	Awaiting description. 
	
	**LLE mode is not available on all platforms**

- **4:3 Resolution** (**320x240**/640x480/960x720/1280x960/1600x1200/1920x1440/2240x1680/2560x1920/2880x2160/3200x2400/3520x2640/3840x2880)

	Select the internal rendering resolution for 4:3 Aspect Ratio mode. The 'Aspect Ratio' core option must be set to 4:3 for this to have an effect.
	
- **16:9 Resolution** (**640x360**/960x540/1280x720/1920x1080/2560x1440/3840x2160/7680x4320)

	Select the internal rendering resolution for 16:9 Aspect Ratio mode. The 'Aspect Ratio' core option must be set to 16:9 or 16:9 adjusted for this to have an effect.

- **Aspect Ratio** (**4:3**/16:9/16:9 adjusted)

	Select the aspect ratio.

- **Bilinear filtering mode** (**standard**/3point)

	Awaiting description.

- **MSAA level** (0/2/4/8/16)

	Awaiting description. 
	
	**This core option is not available on all platforms.**

- **Framebuffer Emulation** (**True**/False)

	Awaiting description.

- **Color buffer to RDRAM** (**Async**/Sync/Off)

	The default setting is dependent on your platform.

- **Depth buffer to RDRAM** (**Software**/FromMem/Off)

	Awaiting description.

- **Hardware per-pixel lighting** (**False**/True)

	Awaiting description.
	
- **Continuous texrect coords** (**Off**/Auto/Force)

	Awaiting description.

- **Native res. 2D texrects** (**False**/True)

	Awaiting description.

- **Less accurate blending mode** (**True**/False)

	Awaiting description.
	
	The default setting is dependent on your platform.

- **GPU shader depth write** (**False/True)

	Awaiting description.
	
	The default seeting is dependent on your platform.

- **Cache GPU Shaders** (**True**/False

	Awaiting description.

- **Crop Mode** (**Auto**/Off)

	Awaiting description.
	
- **Texture filter** (**None**/Smooth filtering 1/Smooth filtering 2/Smooth filtering 3/Smooth filtering 4/Sharp filtering 1/Sharp filtering 2)

	Choose which kind of texture filtering is going to be used.

- **Texture Enhancement** (**None**/As Is/X2/X2SAI/HQ2X/HQ2XS/LQ2X/LQ2XS/HQ4X/2xBRZ/3xBRZ/4xBRZ/5xBRZ/6xBRZ)

	Awaiting description.

- **Filter background textures** (**True**/False)

	Awaiting description.

- **Use High-Res textures** (**False**/True)

	Awaiting description.

- **Use High-Res Full Alpha Channel** (**False**/True)

	Awaiting description.

- **Analog Deadzone (percent)** (**15**/20/25/30/0/5/10)

	Awaiting description.

- **Analog Sensitivity (percent)** (**100**/95/90/85/80/105/110)

	Awaiting description.

- **Right C Button** (**C1**/C2/C3/C4)

	Awaiting description.

- **Left C Button** (**C2/**C3/C4/C1)

	Awaiting description.

- **Down C Button** (**C3**/C4/C1/C2)

	Awaiting description.

- **Up C Button** (**C4**/C1/C2/C3)

	Awaiting description,

- **Player 1 Pak** (**memory**/rumble/none)

	Choose what Pak has been inserted in the player 1 controller.

- **Player 2 Pak** (**none/memory/rumble)

	Choose what Pak has been inserted in the player 2 controller.

- **Player 3 Pak** (**none**/memory/rumble)

	Choose what Pak has been inserted in the player 3 controller.

- **Player 4 Pak** (**none**/memory/rumble)

	Choose what Pak has been inserted in the player 4 controller.

- **Count Per Op** (0/1/2/3)

	Awaiting description.

## Controllers

### Device types

The Mupen64Plus core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 4 device types

- None - Input disabled.
- **Controller** - Joypad

### Rumble support

Rumble only works in the Mupen64Plus core when

- The content being ran has rumble support.
- The joypad input driver being used has rumble support. (e.g. Xinput)
- The joypad device being used has rumble support.
- The 'Player # Pak' core options are set to rumble for the respective players.

[List of Nintendo 64 games with Rumble Pak support](http://nintendo.wikia.com/wiki/List_of_Nintendo_64_games_with_Rumble_Pak_support)

### Controller tables

#### Joypad and analog device type table

| User 1 - 4 Remap descriptors  | RetroPad Inputs                              |
|-------------------------------|----------------------------------------------|
| A Button (C3)                 | ![](images/RetroPad/Retro_B_Round.png)       |
| B Button (C2)                 | ![](images/RetroPad/Retro_Y_Round.png)       |
| START Button                  | ![](images/RetroPad/Retro_Start.png)         |
| Up (digital)                  | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| Down (digital)                | ![](images/RetroPad/Retro_Dpad_Down.png)     |
| Left (digital)                | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| Right (digital)               | ![](images/RetroPad/Retro_Dpad_Right.png)    |
| (C1)                          | ![](images/RetroPad/Retro_A_Round.png)       |
| (C4)                          | ![](images/RetroPad/Retro_X_Round.png)       |
| L-Trigger                     | ![](images/RetroPad/Retro_L1.png)            |
| R-Trigger                     | ![](images/RetroPad/Retro_R1.png)            |
| Z-Trigger                     | ![](images/RetroPad/Retro_L2.png)            | 
| C Buttons Mode                | ![](images/RetroPad/Retro_R2.png)            |
| Control Stick X               | ![](images/RetroPad/Retro_Left_Stick.png) X  |
| Control Stick Y               | ![](images/RetroPad/Retro_Left_Stick.png) Y  |
| C Buttons X                   | ![](images/RetroPad/Retro_Right_Stick.png) X |
| C Buttons Y                   | ![](images/RetroPad/Retro_Right_Stick.png) Y |

## Compatibility

Awaiting description.

## External Links

- [Libretro Mupen64Plus Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/mupen64plus_libretro.info)
- [Libretro Mupen64Plus Github Repository](https://github.com/libretro/mupen64plus-libretro)
- [Report Libretro Mupen64Plus Core Issues Here](https://github.com/libretro/mupen64plus-libretro/issues)
- [Official Mupen64Plus Website](http://www.mupen64plus.org/)
- [Official Mupen64Plus Github Organization](https://github.com/mupen64plus)