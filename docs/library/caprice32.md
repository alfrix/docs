# Amstrad CPC (Caprice32)

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/caprice32.md). Changes are proposed using "Pull Requests."

## Background

Caprice32 is a software emulator of the Amstrad CPC 8bit home computer series running on Linux and Windows. The emulator faithfully imitates the CPC464, CPC664, and CPC6128 models. By recreating the operations of all hardware components at a low level, the emulator achieves a high degree of compatibility with original CPC software. These programs or games can be run unmodified at real-time or higher speeds, depending on the emulator host environment.

### Why use this core?

Awaiting description.

### How to get and install the Caprice32 core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Amstrad CPC (Caprice32)'.

After this has finished downloading, the core should now be ready for use!

### Authors

- Ulrich Doewich
- dantoine

## See also

- [Amstrad CPC (CrocoDS)](https://docs.libretro.com/library/crocods/) - Shared platforms.

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

- [GPLv2](https://github.com/ColinPitrat/caprice32/blob/master/COPYING.txt)

## Extensions

Content that can be loaded by the Caprice32 core have the following file extensions:

- .dsk
- .sna
- .zip
- .tap
- .cdt
- .voc

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✕         |
| States            | ✔         |
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
| Softpatching      | ✕         |
| Disk Control      | ✕         |

### Saves/States

The Caprice32 core's directory name is 'cap32'

Save states can be created in page 2 of the vritual keyboard GUI.

Save states are saved/loaded to and from where the loaded content is.

- .SNA (State)

Content directory

- .SNA (state)


### Virtual Keyboard

The Caprice32 core has a virtual keyboard GUI that can be accessed through the User 1's RetroPad Y input. 

- Here are some actions you can do in page 2 of the vritual keyboard GUI.

- "EXT" EXIT EMU
- "SNA" SAVE SNA
- "DSK" SWITCH DSK DRIVE A/B
- "Col" SWTICH FGCOL ON/OFF

## Core options

The Caprice32 core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.

- **Autorun** (**Off**/On): If enabled, the core will run the first bas/bin found in the DSK.
- **Internal resolution** (**384x272**/400x300): Self-explanatory.
- **Model** (**464**/664/6128): Choose which Amstrad CPC model to emulate.
- **Ram size** (**64**/128/192/512/576): CPC p\hysical RAM size in kB
- **Status Bar** (**Off**/On): Awaiting description.
- **Drive** (**0**/1): Awaiting description.
- **scr_tube** (**Off**/On): Choose between a color display or a monochrome display.

??? note "scr_tube - Off"
	![scr_tube_off](images\Cores\caprice32\scr_tube_off.png)
	
??? note "scr_tube - On"
	![scr_tube_on](images\Cores\caprice32\scr_tube_on.png)	

- **scr_intensity** (**5**/6/7/8/9/10/11/12/13/14/15): Screen cathodic tube intensity

!!! warning ""
	These 'scr_intensity' core option screenshots have been taken with the 'scr_tube' core option set to Off.

??? note "scr_intensity - 5"
	![scr_intensity_5](images\Cores\caprice32\scr_intensity_5.png)
	
??? note "scr_intensity - 15"
	![scr_intensity_!5](images\Cores\caprice32\scr_intensity_15.png)
	
- **Retro joy0** (**Off**/On): Awaiting description.

## Controllers

### Device types

The Caprice32 core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 2 device types

- **RetroPad** - Joypad - **Don't use this, switch to Amstrad Joystick.**
- Amstrad Joystick - Joypad - Optional description.
- Amstrad Keyboard - Keyboard - Optional description.

### Controller tables

#### Joypad and analog device type table

| User 1 input descriptors      | RetroPad                                     | Amstrad Joystick   |
|-------------------------------|----------------------------------------------|--------------------|
| B                             | ![](images/RetroPad/Retro_B_Round.png)       | RUN                |
| Y                             | ![](images/RetroPad/Retro_Y_Round.png)       | VKBD ON/OFF        |
| Select                        | ![](images/RetroPad/Retro_Select.png)        | MOUSE/JOY IN GUI   |
| Start                         | ![](images/RetroPad/Retro_Start.png)         | ENTER/RETURN       |
| Up                            | ![](images/RetroPad/Retro_Dpad_Up.png)       | Joy Up             |
| Down                          | ![](images/RetroPad/Retro_Dpad_Down.png)     | Joy Down           |
| Left                          | ![](images/RetroPad/Retro_Dpad_Left.png)     | Joy Left           |
| Right                         | ![](images/RetroPad/Retro_Dpad_Right.png)    | Joy Right          |
| A                             | ![](images/RetroPad/Retro_A_Round.png)       | FIRE1/VKBD KEY     |
| X                             | ![](images/RetroPad/Retro_X_Round.png)       | FIRE2              |
| L                             | ![](images/RetroPad/Retro_L1.png)            | CAT                |
| R                             | ![](images/RetroPad/Retro_R1.png)            | RESET              |
| L2                            | ![](images/RetroPad/Retro_L2.png)            | STATUS ON/OFF      |
| R2                            | ![](images/RetroPad/Retro_R2.png)            | AUTOLOAD TAPE      |

| User 2 input descriptors      | RetroPad                                     | Amstrad Joystick   |
|-------------------------------|----------------------------------------------|--------------------|
| **                            | ![](images/RetroPad/Retro_B_Round.png)       | -                  |
| **                            | ![](images/RetroPad/Retro_Y_Round.png)       | -                  |
| **                            | ![](images/RetroPad/Retro_Select.png)        | -                  |
| **                            | ![](images/RetroPad/Retro_Start.png)         | -                  |
| **                            | ![](images/RetroPad/Retro_Dpad_Up.png)       | 6	                |
| **                            | ![](images/RetroPad/Retro_Dpad_Down.png)     | 5	  	            |
| **                            | ![](images/RetroPad/Retro_Dpad_Left.png)     | r	                |
| **                            | ![](images/RetroPad/Retro_Dpad_Right.png)    | t                  |
| **                            | ![](images/RetroPad/Retro_A_Round.png)       | g                  |
| **                            | ![](images/RetroPad/Retro_X_Round.png)       | f                  |
| **                            | ![](images/RetroPad/Retro_L1.png)            | -                  |
| **                            | ![](images/RetroPad/Retro_R1.png)            | -                  |
| **                            | ![](images/RetroPad/Retro_L2.png)            | -                  |
| **                            | ![](images/RetroPad/Retro_R2.png)            | -                  |

#### Keyboard device type table

| User 1 - 2 input descriptors  | RetroKeyboard                 | Amstrad Keyboard    |
|-------------------------------|-------------------------------|---------------------|
| **                            | Keyboard Backspace            | Delete              |
| **                            | Keyboard Tab                  | Tab                 |
| **                            | Keyboard Return               | Return              |
| **                            | Keyboard Escape               | Escape              |
| **                            | Keyboard Space                | Space               |
| **                            | Keyboard Comma                | Comma               |
| **                            | Keyboard Period               | Period              |
| **                            | Keyboard 0                    | 0                   |
| **                            | Keyboard 1                    | 1                   |
| **                            | Keyboard 2                    | 2                   |
| **                            | Keyboard 3                    | 3                   |
| **                            | Keyboard 4                    | 4                   |
| **                            | Keyboard 5                    | 5                   |
| **                            | Keyboard 6                    | 6                   |
| **                            | Keyboard 7                    | 7                   |
| **                            | Keyboard 8                    | 8                   |
| **                            | Keyboard 9                    | 9                   |
| **                            | Keyboard Semicolon            | Colon               |
| **                            | Keyboard Equals               | Hat                 |
| **                            | Keyboard Left Bracket         | At                  |
| **                            | Keyboard Right Bracket        | Open Square Bracket |
| **                            | Keyboard a                    | a                   |
| **                            | Keyboard b                    | b                   |
| **                            | Keyboard c                    | c                   |
| **                            | Keyboard d                    | d                   |
| **                            | Keyboard e                    | e                   |
| **                            | Keyboard f                    | f                   |
| **                            | Keyboard g                    | g                   |
| **                            | Keyboard h                    | h                   |
| **                            | Keyboard i                    | i                   |
| **                            | Keyboard j                    | j                   |
| **                            | Keyboard k                    | k                   |
| **                            | Keyboard l                    | l                   | 
| **                            | Keyboard m                    | m                   |  
| **                            | Keyboard n                    | n                   |
| **                            | Keyboard o                    | o                   |
| **                            | Keyboard p                    | p                   |
| **                            | Keyboard q                    | q                   |
| **                            | Keyboard r                    | r                   |
| **                            | Keyboard s                    | s                   |
| **                            | Keyboard t                    | t                   |
| **                            | Keyboard u                    | u                   |
| **                            | Keyboard v                    | v                   |
| **                            | Keyboard w                    | w                   |
| **                            | Keyboard x                    | x                   |
| **                            | Keyboard y                    | y                   |
| **                            | Keyboard z                    | z                   |
| **                            | Keyboard Delete               | Joy Left            |
| **                            | Keyboard Keypad 0             | F0                  |
| **                            | Keyboard Keypad 1             | F1                  |
| **                            | Keyboard Keypad 2             | F2                  |
| **                            | Keyboard Keypad 3             | F3                  |
| **                            | Keyboard Keypad 4             | F4                  |
| **                            | Keyboard Keypad 5             | F5                  |
| **                            | Keyboard Keypad 6             | F6                  |
| **                            | Keyboard Keypad 7             | F7                  |
| **                            | Keyboard Keypad 8             | F8                  |
| **                            | Keyboard Keypad 9             | F9                  |
| **                            | Keyboard Keypad Period        | FDot                |
| **                            | Keyboard Keypad Enter         | Small Enter         |
| **                            | Keyboard Up                   | Cursor Up           |
| **                            | Keyboard Down                 | Cursor Down         |
| **                            | Keyboard Right                | Cursor Right        |
| **                            | Keyboard Left                 | Cursor Left         |
| **                            | Keyboard Insert               | Joy Fire 1          |
| **                            | Keyboard Home                 | Joy Up              |
| **                            | Keyboard End                  | Joy Down            |
| **                            | Keyboard Page Up              | Joy Right           |
| **                            | Keyboard Page Down            | Joy Fire 2          |
| **                            | Keyboard Caps Lock            | Caps Lock           |
| **                            | Keyboard Scroll Lock          | Shift               |
| **                            | Keyboard Left Shift           | Shift               |
| **                            | Keyboard Right Shift          | Control             |
| **                            | Keyboard Left Control         | Control             |
| **                            | Keyboard Left Alt             | Alt                 |
| **                            | Keyboard Right Alt            | Alt                 |
| **                            | Keyboard Compose              | Copy                |

#### Mouse device type table

| User # input descriptors      | RetroMouse                               | In Virtual Keyboard GUI |
|-------------------------------|------------------------------------------|-------------------------|
| **                            | ![](images/RetroMouse/Retro_Mouse.png) X | Mouse X                 |
| **                            | ![](images/RetroMouse/Retro_Mouse.png) Y | Mouse Y                 |
| **                            | ![](images/RetroMouse/Retro_Left.png)    | Click                   |

## External Links

- [Libretro Caprice32 Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/cap32_libretro.info)
- [Libretro Caprice32 Github Repository](https://github.com/libretro/libretro-cap32)
- [Report Libretro Caprice32 Core Issues Here](https://github.com/libretro/libretro-cap32/issues)
- [Official Caprice32 Github Repository](https://github.com/ColinPitrat/caprice32)