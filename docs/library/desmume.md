# Nintendo DS (DeSmuME)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/desmume.md). Changes are proposed using "Pull Requests."

## Background

Port of Desmume to libretro.

### Why use this core?

Awaiting description.

### How to get and install the DeSmuME core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Nintendo DS (DeSmuME)'.

After this has finished downloading, the core should now be ready for use!

#### How to play (after installation):

1. Go back to RetroArch's main menu screen. Select 'Load Content'.

2. Browse to the folder that contains the content you want to run.

3. Select the content that you want to run.

4. If you are asked which core to select, choose 'Nintendo DS (DeSmuME)'.

The game should now start running!

### Authors

- YopYop156
- Zeromus

## See also

- [Nintendo DS (melonDS)](https://docs.libretro.com/library/melonds/) - Shared platforms.

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

- [GPLv2](https://github.com/TASVideos/desmume/blob/master/license.txt)

## Extensions

Content that can be loaded by the DeSmuME core have the following file extensions:

- .nds
- .bin

## Databases

RetroArch database(s) that are associated with the DeSmuME core:

- [Nintendo - Nintendo DS](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Nintendo%20DS.rdb)
- [Nintendo - Nintendo DS Decrypted](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Nintendo%20DS%20Decrypted.rdb)
- [Nintendo - Nintendo DS (Download Play)](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Nintendo%20DS%20(Download%20Play).rdb)

## Features

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
| RetroArch Cheats  | ✔         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| Softpatching      | -         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Crop Overscan     | ✕         |

### Saves/States

The DeSmuME core's directory name is 'DeSmuME'

Game data is saved/loaded to and from where save files are stored.

- .dsv (Game save)

Save states are saved/loaded to and from where state files are stored.

- .state (State)

### Core provided aspect ratio

Awaiting description.

### Nickname

Changing the system nickname isn't currently supported by the DeSmuME core.

## Core options

The DeSmuME core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.

- **Internal resolution (restart)** (**256x192**/512x384/768x576/1024x768/1280x960/1536x1152/1792x1344/2048x1536/2304x1728/2560x1920): 

<center> Self explanatory. Please note that the DeSmuME core is only software rendered.</center>

<center>

??? note "Internal resolution - 256x192"
	![](images\Cores\desmume\256x192.png)
	
</center>

<center>
	
??? note "Internal resolution - 2560x1920"
	![](images\Cores\desmume\2560x1920.png)
	
</center>	

- **CPU cores** (**1**/2/3/4)

<center> Configure how much CPU cores the DeSmuME core will use. Please note that, in general, DeSmuME benefits more from few fast CPUs than from many slow CPUs. For example, a dual-core 3.9GHz CPU will run DeSmuME much faster than a 12-core 1.6GHz CPU. </center>

- **CPU mode** (interpreter/jit)

<center> Choose to run CPU emulation through the Interpreter engine or the JIT Dynamic Recomplier engine. </center>

<center> Interpreter has better compatibility than JIT Dynamic Recompiler. Some games that fail when using JIT Dynamic Recompiler will work fine with Interpreter. The tradeoff here is that Interpreter has much lower performance than JIT Dynamic Recompiler. </center>

<center> Please note that the default setting for this core option is dependent on your hardware. The JIT Dynamic Recompiler is not available on all hardware (e.g. Android devices). </center>

- **JIT block size** (0 to 100 in increments of 1. **12 is default**.)

<center> This core option is only available when the 'CPU mode' core option to set to jit. You may need to tune the block size to prevent some games from breaking. 1 = most accurate, 100 = fastest.</center>

- **Screen layout** (**top/bottom** / bottom/top / left/right / right/left / top only / bottom only / quick switch / hybrid/top / hybrid/bottom)

<center> Self-explanatory. </center>

<center>

??? note "Screen layout - top/bottom"
	![](images\Cores\desmume\top_bottom.png)
	
</center>

<center>

??? note "Screen layout - bottom/top"
	![](images\Cores\desmume\bottom_top.png)
	
</center>

<center>

??? note "Screen layout - left/right"
	![](images\Cores\desmume\left_right.png)
	
</center>

<center>

??? note "Screen layout - right/left"
	![](images\Cores\desmume\right_left.png)
	
</center>

<center>

??? note "Screen layout - top only"
	![](images\Cores\desmume\top.png)
	
</center>

<center>

??? note "Screen layout - bottom only"
	![](images\Cores\desmume\bottom.png)
	
</center>

<center>

??? note "Screen layout - hybrid/top"
	![](images\Cores\desmume\hybrid_top.png)
	
</center>

<center>

??? note "Screen layout - hybrid/bottom"
	![](images\Cores\desmume\hybrid_bottom.png)
	
</center>

- **Hybrid layout scale (restart)** (**1**/3)

<center> Self explanatory. The 'Screen layout' core option must be set to a hybrid setting for this to function properly.</center>

<center>

??? note "Hybrid layout scale - 1"
	![](images\Cores\desmume\scale_1.png)
	
</center>

<center>

??? note "Hybrid layout scale - 3"
	![](images\Cores\desmume\scale_3.png)
	
</center>

- **Hybrid layout show both screens** (Off/**On**)

<center> Removes the small top screen when the 'Screen layout' core option is set to hybrid/top </center>

<center> Removes the small bottom screen when the 'Screen layout' core option is set to hybrid/bottom </center>

- **Hybrid layout cursor always on small screen** (Off/**On**)

<center> Self explanatory. </center>

<center> Disablng this allows you to use the stylus on the big bottom screen when the 'Screen layout' core option is set to hybrid/bottom. </center>

- **Enable mouse/pointer** (Off/**On**)

<center> Enabling this allows you to use mouse inputs for the stylus. </center>

- **Pointer type** (**mouse**/touch)

<center> Setting this to mouse allows you to use mouse inputs for the stylus </center>

<center> Setting this to touch allows you to use touch inputs for the stylus (e.g. Touch controls on Android devices) </center>

- **Pointer Colour** (**white**/black/red/blue/yellow)

<center> Configure the color of the stylus pointer. </center>

<center>

??? note "Pointer Colour - white"
	![](images\Cores\desmume\pointer_white.png)
	
</center>

<center>

??? note "Pointer Colour - black"
	![](images\Cores\desmume\pointer_black.png)
	
</center>

<center>

??? note "Pointer Colour - red"
	![](images\Cores\desmume\pointer_red.png)
	
</center>

<center>

??? note "Pointer Colour - blue"
	![](images\Cores\desmume\pointer_blue.png)
	
</center>

<center>

??? note "Pointer Colour - yellow"
	![](images\Cores\desmume\pointer_yellow.png)
	
</center>

- **Pointer mode l-analog** (**none**/emulated/absolute/pressed)

<center> Awaiting description. </center>

- **Pointer mode r-analog** (**none**/emulated/absolute/pressed)

<center> Awaiting description. </center>

- **Emulated pointer deadzone percent** (0 to 35 in increments of 5. **15 is default**.)

<center> Awaiting description. </center>

- **Emulated pointer acceleration modifier percent** (0 to 100 in increments of 1. **0 is default**.)

<center> Awaiting description. </center>

- **Emulated stylus pressure modifier percent** (0 to 100 in increments of 1. **50 is default**.)

<center> Configure the emulated pressure on the touchscreen from a stylus pressing on it. </center>

- **Enable emulated stylus jitter** (**Off**/On)

<center> Emulate the tiny jitter from a human hand when holding a stylus; some games were accidentally dependent on this. </center>

- **Load Game into Memory (restart)** (**Off**/On)

<center> Loads the entire game into memory before startup. Will decrease in-game loading times at the cost of increased game startup times.</center>

- **Enable Advanced Bus-Level Timing** (Off/**On**)

<center> This will improve or fix some games but it is very performance demanding. Disable this if you want more speed. </center>

- **Firmware language** (**Auto**/English/Japanese/French/German/Italian/Spanish) 

<center> Choose the language of the BIOS. </center>

- **Frameskip** (**0**/1/2/3/4/5/6/7/8/9)

<center> Choose how much frames should be skipped to improve performance at the expense of visual smoothness. </center>

<center> It is generally safe to choose 1 or 2 if you don't mind a slightly choppier game, in order to get a speedup. </center>

<center> If screens seem stuck or screen flickering becomes unacceptable, pick a different frame skip value.  </center>

- **Screen Gap** (0 to 100 in increments of 1. **0 is default.**)

<center> Self explanatory. </center>

<center>

??? note "Screen Gap - 0"
	![](images\Cores\desmume\screengap_0.png)
	
</center>

<center>

??? note "Screen Gap - 100"
	![](images\Cores\desmume\screengap_100.png)
	
</center>

- **Enable Edgemark** (Off/**On**)

<center> Awaiting description. </center>

- **Enable Line Hack** (Off/**On**)

<center> Fixes some graphical bugs involving lines, but causes some other bugs. Not many games use lines. </center>

- **Enable TXT Hack** (**Off**/On)

<center> Fixes text bugs in some games (e.g. Etrian Odyssey). You may need to toggle it off & on by scene. </center>

- **Force Microphone Enable** (**Off**/On)
 
<center> Self explanatory. </center>

- **Microphone Simulation Settings** (**internal**/sample/random/physical): 

<center> Configure microphone input settings. </center>

<center> With the internal setting, DeSmuME will use its internal noise sample for microphone input which works for many games that want you to blow on the mic. </center>

<center> With the sample setting, you can supply your own microphone sample for microphone input. **This may not work currently in the DeSmuME core**. </center>

<center> With the random setting, DeSmuME will use random whitenoise for microphone input which will work for games that require blowing but which don't work with the internal noise sample. </center>

<center> With the physical setting, you can use your default recording device for microphone input. **This may not work currently in the DeSmuME core**. </center>

## Controllers

### Device types

The DeSmuME core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- **RetroPad** - Joypad
- **RetroPad w/Analog** - Joypad - **There is no reason to switch to this.**

### Other controls

### Controller tables

#### Joypad and analog device type table

| User 1 input descriptors      |                                              | RetroPad            |
|-------------------------------|----------------------------------------------|---------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | B                   |
| Y                             | ![](images/RetroPad/Retro_Y_Round.png)       | Y                   | 
| Select                        | ![](images/RetroPad/Retro_Select.png)        | Select              |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | Start               |
| Up                            | ![](images/RetroPad/Retro_Dpad_Up.png)       | Up                  |
| Down                          | ![](images/RetroPad/Retro_Dpad_Down.png)     | Down                |
| Left                          | ![](images/RetroPad/Retro_Dpad_Left.png)     | Left                |
| Right                         | ![](images/RetroPad/Retro_Dpad_Right.png)    | Right               |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | A                   |
| X                             | ![](images/RetroPad/Retro_X_Round.png)       | X                   |
| L                             | ![](images/RetroPad/Retro_L1.png)            | L                   |
| R                             | ![](images/RetroPad/Retro_R1.png)            | R                   |
| Lid Close/Open                | ![](images/RetroPad/Retro_L2.png)            | Lid Close/Op        |
| Tap Stylus                    | ![](images/RetroPad/Retro_R2.png)            | Tap Stylus          |
| Toggle Microphone             | ![](images/RetroPad/Retro_L3.png)            | Toggle Microphone   |
| Quick Screen Switch           | ![](images/RetroPad/Retro_R3.png)            | Quick Screen Switch |
| N/A                           | ![](images/RetroPad/Retro_Left_Stick.png) X  | [Pointer mode l-analog](https://buildbot.libretro.com/.docs/library/desmume/#core-options) |
| N/A                           | ![](images/RetroPad/Retro_Left_Stick.png) Y  | [Pointer mode l-analog](https://buildbot.libretro.com/.docs/library/desmume/#core-options) |
| N/A                           | ![](images/RetroPad/Retro_Right_Stick.png) X | [Pointer mode r-analog](https://buildbot.libretro.com/.docs/library/desmume/#core-options) |
| N/A                           | ![](images/RetroPad/Retro_Right_Stick.png) Y | [Pointer mode r-analog](https://buildbot.libretro.com/.docs/library/desmume/#core-options) |

#### Mouse device type table

| User 1 input descriptors      |                                          | Stylus             |
|-------------------------------|------------------------------------------|--------------------|
| N/A                           | ![](images/RetroMouse/Retro_Mouse.png)   | Stylus             |
| N/A                           | ![](images/RetroMouse/Retro_Left.png)    | Press              |

#### Pointer device type table

| User 1 input descriptors      |                 | Stylus             |
|-------------------------------|-----------------|--------------------|
| N/A                           | Pointer         | Stylus             |
| N/A                           | Pointer Pressed | Press              |

## External Links

- [Libretro DeSmuME Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/desmume_libretro.info)
- [Libretro DeSmuME Github Repository](https://github.com/libretro/desmume)
- [Report Libretro DeSmuME Core Issues Here](https://github.com/libretro/desmume/issues)
- [Official DeSmuME Website](https://desmume.org/)
- [Official DeSmuME Github Repository](https://github.com/TASVideos/desmume)