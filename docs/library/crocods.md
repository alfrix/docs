# Amstrad CPC (CrocoDS)

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/crocods.md). Changes are proposed using "Pull Requests."

## Background

Based on Win-CPC. CrocoDS was originally an Amstrad CPC emulator created for the Nintendo DS and was ported to libretro some time after.

### Why use this core?

Awaiting description.

### How to get and install the CrocoDS core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'Amstrad CPC (CrocoDS)'.

After this has finished downloading, the core should now be ready for use!

### Authors

- RedBug

## See also

- [Amstrad CPC (Caprice32)](https://buildbot.libretro.com/docs/library/caprice32/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://buildbot.libretro.com/docs/tech/licenses/).

- [MIT](https://github.com/libretro/libretro-crocods/blob/master/LICENSE)

## Extensions

Content that can be loaded by the CrocoDS core have the following file extensions:

- dsk
- sna
- [kcr](https://github.com/redbug26/crocods-core/wiki/kcr)

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
| Softpatching      | ✕         |

### Saves/States

The CrocoDS core's directory name is 'crocods'

Save states are saved/loaded to and from where state files are stored.

- .state

State directory

- .state ()

## Core options

The CrocoDS core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.

- **Color Monitor** (**color**/green): Self-explanatory.

??? note "Color Monitor - color"
	![color_monitor_color](images\Cores\crocods\color_monitor_color.png)
	
??? note "Color Monitor - green"
	![color_monitor_green](images\Cores\crocods\color_monitor_green.png)	

- **Resize** (**Auto**/320x200/Overscan): Self-explanatory.

??? note "Resize - 320x200"
	![screenshot_name](images\Cores\crocods\resize_320x200.png)
	
??? note "Resize - Overscan"
	![screenshot_name](images\Cores\crocods\resize_overscan.png)	

- **Speed hack** (**no**/yes): Awaiting description.

## Controllers

### Device types

The CrocoDS core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- **RetroPad** - Joypad - Look at the User 1 RetroPad graph below for inputs.
- RetroKeyboard - Keyboard  - Awaiting description.

#### User 2 device types

- **RetroPad** - Joypad - Look at the User 2 RetorPad graph below for inputs.
- RetroKeyboard - Keyboard  - Awaiting description.

### Controllers graph

| CrocoDS     | User 1 RetroPad                            |
|-------------|--------------------------------------------|
| Joy Fire 2  | ![](images/RetroPad/Retro_B_Round.png)     |
| Space       | ![](images/RetroPad/Retro_Select.png)      |
| Return      | ![t](images/RetroPad/Retro_Start.png)      |
| Joy Up      | ![](images/RetroPad/Retro_Dpad_Up.png)     |
| Joy Down    | ![](images/RetroPad/Retro_Dpad_Down.png)   |
| Joy Left    | ![](images/RetroPad/Retro_Dpad_Left.png)   |
| Joy Right   | ![](images/RetroPad/Retro_Dpad_Right.png)  |
| Joy Fire 2  | ![](images/RetroPad/Retro_A_Round.png)     |

| CrocoDS      | User 2 RetroPad                            |
|--------------|--------------------------------------------|
| Space        | ![](images/RetroPad/Retro_B_Round.png)     |
| Space        | ![](images/RetroPad/Retro_Select.png)      |
| Return       | ![t](images/RetroPad/Retro_Start.png)      |
| Cursor Up    | ![](images/RetroPad/Retro_Dpad_Up.png)     |
| Cursor Down  | ![](images/RetroPad/Retro_Dpad_Down.png)   |
| Cursor Left  | ![](images/RetroPad/Retro_Dpad_Left.png)   |
| Cursor Right | ![](images/RetroPad/Retro_Dpad_Right.png)  |
| Space        | ![](images/RetroPad/Retro_A_Round.png)     |

| CrocoDS             | RetroKeyboard                                                                  |
|---------------------|--------------------------------------------------------------------------------|
| 0     			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_0.png)             |
| 1     			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_1.png)             |
| 2     			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_2.png)             |
| 3     			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_3.png)             |
| 4     			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_4.png)             |
| 5      			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_5.png)             |
| 6     			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_6.png)             |
| 7     			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_7.png)             |
| 8     			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_8.png)             |
| 9      		      | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_9.png)             |
| A      			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_A.png)             |
| B      			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_B.png)             |
| C      	          | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_C.png)             |
| D      			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_D.png)             |
| E      			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_E.png)             |
| F      			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_F.png)             |
| G      			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_G.png)             |
| H       			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_H.png)             |
| I       			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_I.png)             |
| J       			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_J.png)             |
| K       			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_K.png)             |
| L       			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_L.png)             |
| M       			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_M.png)             |
| N       			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_N.png)             |
| O       		      | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_O.png)             |
| P        			  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_P.png)             |
| Q                   | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Q.png)             |
| R                   | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_R.png)             |
| S                   | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_S.png)             |
| T                   | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_T.png)             |
| U                   | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_U.png)             |
| V                   | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_V.png)             |
| W                   | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_W.png)             |
| X                   | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_X.png)             |
| Y                   | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Y.png)             |
| Z                   | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Z.png)             |
| Space               | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Space.png)         |
| Comma               | Comma                                                                          |
| Dot                 | Period                                                                         |
| Colon               | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Semicolon.png)     |
| Minus               | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Minus.png)         |
| Hat                 | Equals                                                                         |
| At                  | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Bracket_Left.png)  |
| Open Square Bracket | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Bracket_Right.png) |
| Tab                 | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Tab.png)           |
| Return              | Return                                                                         |
| Delete              | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Backspace.png)     |
| Escape              | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Esc.png)           |
| Cursor Up           | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Arrow_Up.png)      |
| Cursor Down         | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Arrow_Down.png)    |
| Cursor Left         | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Arrow_Left.png)    |
| Cursor Right        | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Arrow_Right.png)   |
| F0                  | Keypad 0                                                                       |
| F1                  | Keypad 1                                                                       |
| F2                  | Keypad 2                                                                       |
| F3                  | Keypad 3                                                                       |
| F4                  | Keypad 4                                                                       |
| F5                  | Keypad 5                                                                       |
| F6                  | Keypad 6                                                                       |
| F7                  | Keypad 7                                                                       |
| F8                  | Keypad 8                                                                       |
| F9                  | Keypad 9                                                                       |
| Fdot                | Keypad Period                                                                  |
| Shift               | Left Shift                                                                     |
| Shift               | Right Shift                                                                    |
| Control             | Left Control                                                                   |
| Control             | Right Control                                                                  |
| Caps Lock           | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Caps_Lock.png)     |
| Small Enter         | Keypad Enter                                                                   |
| Joy Left            | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Del.png)        |
| Joy Right           | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Page_Down.png)     |
| Joy Up              | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Home.png)          |
| Joy Down            | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_End.png)           |
| Joy Fire 1          | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Insert.png)           |
| Joy Fire 2          | ![](images/Button_Pack/Keyboard_&_Mouse/Dark/Keyboard_Black_Page_Up.png)       |

## External Links

- [Libretro CrocoDS Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/crocods_libretro.info)
- [Libretro CrocoDS Github Repository](https://github.com/libretro/libretro-crocods)
- [Report Libretro CrocoDS Core Issues Here](https://github.com/libretro/libretro-crocods/issues)
- [Official CrocoDS Github Repository](https://github.com/redbug26/crocods-core)