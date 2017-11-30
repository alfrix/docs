# Game Boy/Game Boy Color (SameBoy)

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/sameboy.md). Changes are proposed using "Pull Requests."

## Background

SameBoy is an extremely accurate open source Gameboy (DMG) and Gameboy Color (CGB) emulator, written in portable C.

### Why use this core?

Awaiting description.

### How to get and install the SameBoy core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Game Boy/Game Boy Color (SameBoy)'.

4. After this has finished downloading, the core should now be ready for use!

### Authors

- LIJI32

## See also

- [Game Boy / Game Boy Color (Emux)](https://doc.libretro.com/library/emux_gb/)
- [Game Boy / Game Boy Color (Gambatte)](https://doc.libretro.com/library/gambatte/)
- [Game Boy / Game Boy Color (TGB Dual)](https://doc.libretro.com/library/tgbdual/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://buildbot.libretro.com/docs/tech/licenses/).

- [MIT](https://github.com/libretro/SameBoy/blob/master/LICENSE)

## Extensions

Content that can be loaded by the SameBoy core have the following file extensions:

- .gb
- .gbc

## Databases

RetroArch database(s) that are associated with the SameBoy core:

- [Nintendo - Game Boy](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy.rdb)
- [Nintendo - Game Boy Color](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Game%20Boy%20Color.rdb)

## BIOS

Required or optional firmware files go in RetroArch's system directory.

!!! warning ""
	The SameBoy core has reverse engineered Game Boy/Game Boy Color boot ROMs baked into the core itself so real BIOS files aren't required. If you’d like to override this, you can place the following BIOS files in RetroArch's system directory.

|   Filename   |      Description                   |              md5sum              |
|:------------:|:----------------------------------:|:--------------------------------:|
| dmg_boot.bin | Game Boy boot ROM - Optional       | 32fbbd84168d3482956eb3c5051637f5 |
| cgb_boot.bin | Game Boy Color boot ROM - Optional | dbfce9db9deaa2567f6a84fde55f9680 |

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| RetroAchievements | ✔         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controllers       | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | ✕         |
| Rumble            | ✔         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| Softpatching      | ✕         |

### Saves/States

The SameBoy core's directory name is 'SameBoy'

Game data is saved/loaded to and from where save files are stored.

- .srm (Battery save)
- .rtc (Real Time Clock save)

Save states are saved/loaded to and from where state files are stored.

- .state (State)

### Rumble

Rumble only works when the joypad input driver being used has rumble function implementation (e.g. **Xinput**).

## Core options

The SameBoy core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.

- **Color Correction** (**off**/correct curves/emulate hardware/preserve brightness): Self-explanatory. **Only for Gameboy Color games**

??? note "Color Correction - off"
	![](images\Cores\sameboy\color_off.png)
	
??? note "Color Correction - correct curves"
	![](images\Cores\sameboy\color_curves.png)

??? note "Color Correction - emulate hardware"
	![](images\Cores\sameboy\color_hardware.png)

??? note "Color Correction - preserve brightness"
	![](images\Cores\sameboy\color_brightness.png)

- **High Pass Filter** (**off**/accurate/remove dc offset): Awaiting description.

## Controllers

The SameBoy core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):

### User 1 - 2 Device Types

- **RetroPad** - Joypad
- **Nintendo Gameboy** - Joypad

### User 3 - 16 Device Types

- **RetroPad** - Joypad

### Controllers graph

| SameBoy     | RetroPad                                  |
|-------------|-------------------------------------------|
| B           | ![](images/RetroPad/Retro_B_Round.png)    |
| Select      | ![](images/RetroPad/Retro_Select.png)     |
| Start       | ![](images/RetroPad/Retro_Start.png)      |
| Up          | ![](images/RetroPad/Retro_Dpad_Up.png)    |
| Down        | ![](images/RetroPad/Retro_Dpad_Down.png)  |
| Left        | ![](images/RetroPad/Retro_Dpad_Left.png)  |
| Right       | ![](images/RetroPad/Retro_Dpad_Right.png) |
| A           | ![](images/RetroPad/Retro_A_Round.png)    |

## External Links

- [Libretro SameBoy Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/sameboy_libretro.info)
- [Libretro SameBoy Github Repository](https://github.com/libretro/SameBoy)
- [Report Libretro SameBoy Core Issues Here](https://github.com/libretro/libretro-meta/issues)
- [Official SameBoy Website](https://sameboy.github.io/)
- [Official SameBoy Github Repository](https://github.com/LIJI32/SameBoy)