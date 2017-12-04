# (Title)

// Copy the display name entry in the core info file and paste it here for the title.
// https://github.com/libretro/libretro-super/tree/master/dist/info

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/). Changes are proposed using "Pull Requests."

// Add (core-doc-filename).md to the end of the URL.

## Background

Awaiting description.

// Put background information for the core here.

### Why use this core?
// Optional section.

Awaiting description.

// This section is for platforms that have multiple libretro cores like the SNES.

// Possible topics to talk about.
/// Does the core have notable enhancements or differences compared to standalone or other cores?
/// Is the core recommended for netplay?
/// Is the core designed to run on specific hardware or platforms?
/// Is the core recommended for romhacks?

### How to get and install the (Core name) core:

// Fill in the (Core name).

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select '(Title)'.

// Fill in the (Title).

After this has finished downloading, the core should now be ready for use!

#### How to play (after installation):
// Optional section.
// This section is for cores that need files from RetroArch's content downloader.

1. Go back to RetroArch's main menu screen. Select 'Load Content', then 'Downloads'.

2. Select the '(Content directory name)' directory, then select '(Game filename)'.

// Fill in the (Content directory name) and the (Game filename).

3. If you are asked which core to select, choose '(Title)'.

// Fill in the title.

The game should now start running!

#### How to play (after installation):
// Optional section.
// This section is for cores that don't need any content to be started.

1. Go back to RetroArch's main menu screen. Select 'Load Core', then '(Core name)'.

// Fill in the (Core name).

2. Now, select 'Start Core'.

The game should now start running!

### Authors

- (Author)

// Copy the author entry in the core info file and paste it here.
// https://github.com/libretro/libretro-super/tree/master/dist/info

## See also
// Optional section.

- [Other Core](https://buildbot.libretro.com/docs/library/) - Optional description.

// Add links to related core docs here.

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://buildbot.libretro.com/docs/tech/licenses/).

- [license](https://link)

// Copy the license entry in the core info file and a url to license information and paste it here.
//(https://github.com/libretro/libretro-super/tree/master/dist/info)

## Extensions
// Optional section.

Content that can be loaded by the (Core name) core have the following file extensions:

// Fill in the (Core name).

- .(extension)

// Copy the exntension entry in the core info file and paste it here.
// https://github.com/libretro/libretro-super/tree/master/dist/info)

## Databases
// Optional section.

RetroArch database(s) that are associated with the (Core name) core:

// Fill in the (Core name).

- (Database name)[Database file URL]

// Copy the database entry in the core info file and paste it here. Also, paste in the link for the database. 
// https://github.com/libretro/libretro-super/tree/master/dist/info
// https://github.com/libretro/libretro-database/tree/master/rdb

## BIOS
// Optional section.

Required or optional firmware files go in RetroArch's system directory.

|   Filename    |    Description         |              md5sum              |
|:-------------:|:----------------------:|:--------------------------------:|
| optional.bin  | Description - Optional |                                  |
| required.bin  | Description - Required |                                  |

// Copy the firmware information in the ccore info file and paste it here (
// https://github.com/libretro/libretro-super/tree/master/dist/info)--

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | -         |
| States            | -         |
| Rewind            | -         |
| Netplay           | -         |
| RetroAchievements | -         |
| RetroArch Cheats  | -         |
| Native Cheats     | -         |
| Controllers       | -         |
| Remapping         | -         |
| Multi-Mouse       | -         |
| Rumble            | -         |
| Sensors           | -         |
| Camera            | -         |
| Location          | -         |
| Subsystem         | -         |
| Softpatching      | -         |
| Crop Overscan     | -         |
| Username          | -         |
| Disk Control      | -         |

// Use ✔ or ✕
// Leave it as - if unsure.

### Saves/States

The (Core name) core's directory name is '(Directory name)'

// Fill in the (Core name) and the (Directory name).
// The (Directory name) is the name of the directory the core creates in RetroArch's save and state directories.

Game data is saved/loaded to and from where save files are stored.

- .srm (Save data)

Save states are saved/loaded to and from where state files are stored.

- .state (State)

// Add a list of files the core saves and loads from its directories. 

### Core provided aspect ratio

## Core options
// Optional section.

The (Core name) core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.

// Fill in the (Core name).

- **Core Option** (**Setting1**/Setting2): Awaiting description.

// Fill in core options.

??? note "Core Option - Setting"
	![](images\Cores\folder\screenshot_name.png)
	
// Add core option screenshots if needed.
	
## Controllers

### Device types

The (Core name) core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

// Fill in the (Core name).

#### User # - # device types

- **(Device type name)** - (Device type) - Optional description.

// Fill in (Device type name).

// Fill in (Device type)
/// Possible device types
//// None
//// Joypad
//// Analog
//// Keyboard
//// Mouse
//// Lightgun
//// Pointer

### Controller tables

#### Joypad and analog device type table

| (Core Name) input descriptors | RetroPad                                     | (Device type name) |
|-------------------------------|----------------------------------------------|--------------------|
| Action 1                      | ![](images/RetroPad/Retro_B_Round.png)       | -                  |
| Action 2                      | ![](images/RetroPad/Retro_Y_Round.png)       | -                  |
| Action 3                      | ![](images/RetroPad/Retro_Select.png)        | -                  |
| Action 4                      | ![](images/RetroPad/Retro_Start.png)         | -                  |
| Action 5                      | ![](images/RetroPad/Retro_Dpad_Up.png        | -                  |
| Action 6                      | ![](images/RetroPad/Retro_Dpad_Down.png      | -                  |
| Action 7                      | ![](images/RetroPad/Retro_Dpad_Left.png      | -                  |
| Action 8                      | ![](images/RetroPad/Retro_Dpad_Right.png     | -                  |
| Action 9                      | ![](images/RetroPad/Retro_A_Round.png)       | -                  |
| Action 10                     | ![](images/RetroPad/Retro_X_Round.png)       | -                  |
| Action 11                     | ![](images/RetroPad/Retro_L1.png)            | -                  |
| Action 12                     | ![](images/RetroPad/Retro_R2.png)            | -                  |
| Action 13                     | ![](images/RetroPad/Retro_L2.png)            | -                  |
| Action 14                     | ![](images/RetroPad/Retro_R2.png)            | -                  |
| Action 15                     | ![](images/RetroPad/Retro_L3.png)            | -                  |
| Action 16                     | ![](images/RetroPad/Retro_R3.png)            | -                  |
| Action 17                     | ![](images/RetroPad/Retro_Left_Stick.png) X  | -                  |
| Action 18                     | ![](images/RetroPad/Retro_Left_Stick.png) Y  | -                  |
| Action 19                     | ![](images/RetroPad/Retro_Right_Stick.png) X | -                  |
| Action 20                     | ![](images/RetroPad/Retro_Right_Stick.png) Y | -                  |

#### Keyboard device type table

| (Core name) input descriptors | RetroKeyboard                 | (Device type name) |
|-------------------------------|-------------------------------|--------------------|
| Action 1                      | Keyboard Backspace            | -                  |
| Action 2                      | Keyboard Tab                  | -                  |
| Action 3                      | Keyboard Clear                | -                  |
| Action 4                      | Keyboard Return               | -                  |
| Action 5                      | Keyboard Pause                | -                  |
| Action 6                      | Keyboard Escape               | -                  |
| Action 7                      | Keyboard Space                | -                  |
| Action 8                      | Keyboard Exclaimation         | -                  |
| Action 9                      | Keyboard Double Quote         | -                  |
| Action 10                     | Keyboard Hash                 | -                  |
| Action 11                     | Keyboard Dollar               | -                  |
| Action 12                     | Keyboard Ampersand            | -                  |
| Action 13                     | Keyboard Quote                | -                  |
| Action 14                     | Keyboard Left Parentheses     | -                  |
| Action 15                     | Keyboard Right Parentheses    | -                  |
| Action 16                     | Keyboard Asterisk             | -                  |
| Action 17                     | Keyboard Plus                 | -                  |
| Action 18                     | Keyboard Comma                | -                  |
| Action 19                     | Keyboard Minus                | -                  |
| Action 20                     | Keyboard Period               | -                  |
| Action 21                     | Keyboard Slash                | -                  |
| Action 22                     | Keyboard 0                    | -                  |
| Action 23                     | Keyboard 1                    | -                  |
| Action 24                     | Keyboard 2                    | -                  |
| Action 25                     | Keyboard 3                    | -                  |
| Action 25                     | Keyboard 4                    | -                  |
| Action 26                     | Keyboard 5                    | -                  |
| Action 27                     | Keyboard 6                    | -                  |
| Action 28                     | Keyboard 7                    | -                  |
| Action 29                     | Keyboard 8                    | -                  |
| Action 30                     | Keyboard 9                    | -                  |
| Action 31                     | Keyboard Colon                | -                  |
| Action 32                     | Keyboard Semicolon            | -                  |
| Action 33                     | Keyboard Less than            | -                  |
| Action 34                     | Keyboard Equals               | -                  |
| Action 35                     | Keyboard Greater              | -                  |
| Action 36                     | Keyboard Question             | -                  |
| Action 37                     | Keyboard At                   | -                  |
| Action 38                     | Keyboard Left Bracket         | -                  |
| Action 39                     | Keyboard Backslash            | -                  |
| Action 40                     | Keyboard Right Bracket        | -                  |
| Action 41                     | Keyboard Caret                | -                  |
| Action 42                     | Keyboard Underscore           | -                  |
| Action 43                     | Keyboard Backquote            | -                  |
| Action 44                     | Keyboard a                    | -                  |
| Action 45                     | Keyboard b                    | -                  |
| Action 46                     | Keyboard c                    | -                  |
| Action 47                     | Keyboard d                    | -                  |
| Action 48                     | Keyboard e                    | -                  |
| Action 49                     | Keyboard f                    | -                  |
| Action 50                     | Keyboard g                    | -                  |
| Action 51                     | Keyboard h                    | -                  |
| Action 52                     | Keyboard i                    | -                  |
| Action 53                     | Keyboard j                    | -                  |
| Action 54                     | Keyboard k                    | -                  |
| Action 55                     | Keyboard l                    | -                  |
| Action 56                     | Keyboard m                    | -                  |
| Action 57                     | Keyboard n                    | -                  |
| Action 57                     | Keyboard o                    | -                  |
| Action 58                     | Keyboard p                    | -                  |
| Action 59                     | Keyboard q                    | -                  |
| Action 60                     | Keyboard r                    | -                  |
| Action 61                     | Keyboard s                    | -                  |
| Action 62                     | Keyboard t                    | -                  |
| Action 63                     | Keyboard u                    | -                  |
| Action 64                     | Keyboard v                    | -                  |
| Action 65                     | Keyboard w                    | -                  |
| Action 66                     | Keyboard x                    | -                  |
| Action 67                     | Keyboard y                    | -                  |
| Action 68                     | Keyboard z                    | -                  |
| Action 69                     | Keyboard Delete               | -                  |
| Action 70                     | Keyboard Keypad 0             | -                  |
| Action 71                     | Keyboard Keypad 1             | -                  |
| Action 72                     | Keyboard Keypad 2             | -                  |
| Action 73                     | Keyboard Keypad 3             | -                  |
| Action 74                     | Keyboard Keypad 4             | -                  |
| Action 75                     | Keyboard Keypad 5             | -                  |
| Action 76                     | Keyboard Keypad 6             | -                  |
| Action 77                     | Keyboard Keypad 7             | -                  |
| Action 78                     | Keyboard Keypad 8             | -                  |
| Action 79                     | Keyboard Keypad 9             | -                  |
| Action 80                     | Keyboard Keypad Period        | -                  |
| Action 81                     | Keyboard Keypad Divide        | -                  |
| Action 82                     | Keyboard Keypad Multiply      | -                  |
| Action 83                     | Keyboard Keypad Minus         | -                  |
| Action 84                     | Keyboard Keypad Plus          | -                  |
| Action 85                     | Keyboard Keypad Enter         | -                  |
| Action 86                     | Keyboard Keypad Equals        | -                  |
| Action 87                     | Keyboard Up                   | -                  |
| Action 88                     | Keyboard Down                 | -                  |
| Action 89                     | Keyboard Right                | -                  |
| Action 90                     | Keyboard Left                 | -                  |
| Action 100                    | Keyboard Insert               | -                  |
| Action 101                    | Keyboard Home                 | -                  |
| Action 102                    | Keyboard End                  | -                  |
| Action 103                    | Keyboard Page Up              | -                  |
| Action 104                    | Keyboard Page Down            | -                  |
| Action 105                    | Keyboard F1                   | -                  |
| Action 106                    | Keyboard F2                   | -                  |
| Action 107                    | Keyboard F3                   | -                  |
| Action 108                    | Keyboard F4                   | -                  |
| Action 109                    | Keyboard F5                   | -                  |
| Action 110                    | Keyboard F6                   | -                  |
| Action 111                    | Keyboard F7                   | -                  |
| Action 112                    | Keyboard F8                   | -                  |
| Action 113                    | Keyboard F9                   | -                  |
| Action 114                    | Keyboard F10                  | -                  |
| Action 115                    | Keyboard F11                  | -                  |
| Action 116                    | Keyboard F12                  | -                  |
| Action 117                    | Keyboard F13                  | -                  |
| Action 118                    | Keyboard F14                  | -                  |
| Action 119                    | Keyboard F15                  | -                  |
| Action 120                    | Keyboard Num Lock             | -                  |
| Action 121                    | Keyboard Caps Lock            | -                  |
| Action 122                    | Keyboard Scroll Lock          | -                  |
| Action 123                    | Keyboard Left Shift           | -                  |
| Action 124                    | Keyboard Right Shift          | -                  |
| Action 125                    | Keyboard Left Control         | -                  |
| Action 126                    | Keyboard Left Alt             | -                  |
| Action 127                    | Keyboard Right Alt            | -                  |
| Action 128                    | Keyboard Left Meta            | -                  |
| Action 129                    | Keyboard Right Meta           | -                  |
| Action 130                    | Keyboard Left Super           | -                  |
| Action 131                    | Keyboard Right Super          | -                  |
| Action 132                    | Keyboard Modifier Shift       | -                  |
| Action 133                    | Keyboard Modifier Control     | -                  |
| Action 134                    | Keyboard Modifier Alt         | -                  |
| Action 135                    | Keyboard Modifier Meta        | -                  |
| Action 136                    | Keyboard Modifier Num Lock    | -                  |
| Action 137                    | Keyboard Modifier Caps Lock   | -                  |
| Action 138                    | Keyboard Modifier Scroll Lock | -                  |
| Action 139                    | Keyboard Mode                 | -                  |
| Action 140                    | Keyboard Compose              | -                  |
| Action 141                    | Keyboard Help                 | -                  |
| Action 142                    | Keyboard Print                | -                  |
| Action 143                    | Keyboard System Request       | -                  |
| Action 144                    | Keyboard Break                | -                  |
| Action 145                    | Keyboard Menu                 | -                  |
| Action 146                    | Keyboard Power                | -                  |
| Action 147                    | Keyboard Euro                 | -                  |
| Action 148                    | Keyboard Undo                 | -                  |

#### Mouse device type table

| (Core Name) input descriptors | RetroMouse                               | (Device type name) |
|-------------------------------|------------------------------------------|--------------------|
| Action 1                      | ![](images/RetroMouse/Retro_Mouse.png) X | -                  |
| Action 2                      | ![](images/RetroMouse/Retro_Mouse.png) Y | -                  |
| Action 3                      | ![](images/RetroMouse/Retro_Left.png)    | -                  |
| Action 4                      | ![](images/RetroMouse/Retro_Right.png)   | -                  |
| Action 5                      | Mouse Wheel Up                           | -                  |
| Action 6                      | Mouse Wheel Down                         | -                  |
| Action 7                      | ![](images/RetroMouse/Retro_Middle.png)  | -                  |
| Action 8                      | Mouse Horizontal Wheel Up                | -                  |
| Action 9                      | Mouse Horizontal Wheel Down              | -                  |
| Action 10                     | Mouse Button 4                           | -                  |
| Action 11                     | Mouse Button 5                           | -                  |

#### Lightgun device type table

| (Core Name) input descriptors | RetroLightgun   | (Device type name) |
|-------------------------------|-----------------|--------------------|
| Action 1                      | Gun X           | -                  |
| Action 2                      | Gun Y           | -                  |
| Action 2                      | Gun Trigger     | -                  |
| Action 3                      | Gun Reload      | -                  |
| Action 4                      | Gun Aux A       | -                  |
| Action 5                      | Gun Aux B       | -                  |
| Action 6                      | Gun Aux C       | -                  |
| Action 7                      | Gun Start       | -                  |
| Action 8                      | Gun Select      | -                  |
| Action 9                      | Gun D-pad Up    | -                  |
| Action 10                     | Gun D-pad Down  | -                  |
| Action 11                     | Gun D-pad Left  | -                  |
| Action 12                     | Gun D-pad Right | -                  |

#### Pointer device type table

| (Core Name) input descriptors | RetroPointer    | (Device type name) |
|-------------------------------|-----------------|--------------------|
| Action 1                      | Pointer X       | -                  |
| Action 2                      | Pointer Y       | -                  |
| Action 3                      | Pointer Pressed | -                  |

// Fill in the (Core name) in the device type tables that will be used.
// Fill out the device type tables that will be used,.

## Compatibility
// Optional section.

// Paste in a link to a compatibility list.
- [(Core name) Compatibility List](URL)

// Or write up a compatibility description.
Awaiting description.

// Or make a compatibility table.
| Game | Issue |
|------|-------|
|      |       |

## External Links

// Put relevant links here.
- [Libretro (Core name) Core info file](https://link)
- [Libretro (Core name) (Website name) Repository](https://link)
- [Report Libretro (Core name) Core Issues Here](https://link)
- [Official (Core name) Website](https://link)
- [Official (Core name) (Website name) Repository](https://link)