# Cave Story (NXEngine)

## Contribute to this documentation

In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/nxengine.md). Changes are proposed using "Pull Requests."

There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)

You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).

## Background

NXEngine is a open source reproduction of the [Cave Story game engine](https://en.wikipedia.org/wiki/Cave_Story).

### Why use this core?

Awaiting description.

### How to get and install the NXEngine core:

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

2. Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

3. Browse through the list and select 'Cave Story (NXEngine)'.

<center> ![](images\Cores\nxengine\nxengine.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

1. You now need to obtain NXEngine's data files. You can do this by going back to the previous menu screen. From there, select 'Content Downloader'.

<center> ![](images\Cores\all\download.png) </center>

2. Select 'NXEngine', then select 'Cave Story (En).zip'. This should download and extract this file to RetroArch's Downloads directory.

<center> ![](images\Cores\nxengine\down_story.png) </center>

3. Go back to RetroArch's main menu screen. Select 'Load Content', then 'Downloads'.

<center> ![](images\Cores\all\load.png) </center>

<center> ![](images\Cores\all\downloads.png) </center>

4. Select the 'Cave Story (en)' directory, then select 'Doukutsu.exe'.

<center> ![](images\Cores\nxengine\doukutsu.png) </center>

5. If you are asked which core to select, choose 'NXEngine'.

The content should now start running!

### Authors

- Caitlin Shaw

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The NXEngine core is licensed under

- [GPLv3](https://github.com/gameblabla/nxengine-nspire/blob/master/LICENSE)

## Extensions

Content that can be loaded by the NXEngine core have the following file extensions:

- .exe

## Databases

RetroArch database(s) that are associated with the NXEngine core:

- [Cave Story](https://github.com/libretro/libretro-database/blob/master/rdb/Cave%20Story.rdb)

## Features

RetroArch-level settings or features that the NXEngine core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✕         |
| Rewind            | ✕         |
| Netplay           | ✕         |
| Core Options      | ✕         |
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

The NXEngine core's directory name is 'NXEngine'

The NXEngine core saves/loads to/from these directories.

**RetroArch's Save directory**

- profile#.dat (Save data profile)

### Geometry and timing

- The NXEngine core's internal FPS is 60
- The NXEngine core's internal sample rate is 22050 Hz
- The NXEngine core's core provided aspect ratio is (Ratio)

## Controllers

### Device types

The NXEngine core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 device types

- None - Doesn't disable input
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There is no reason to switch to this.

### Controller tables

#### Joypad and analog device type table

| User 1 Input descriptors      | RetroPad Inputs                              |
|-------------------------------|----------------------------------------------|
| Jump                          | ![](images/RetroPad/Retro_B_Round.png)       |
| Settings                      | ![](images/RetroPad/Retro_Select.png)        |
| Inventory                     | ![](images/RetroPad/Retro_Start.png)         |
| D-Pad Up                      | ![](images/RetroPad/Retro_Dpad_Up.png)       |
| D-Pad Down                    | ![](images/RetroPad/Retro_Dpad_Down.png)     |
| D-Pad Left                    | ![](images/RetroPad/Retro_Dpad_Left.png)     |
| D-Pad Right                   | ![](images/RetroPad/Retro_Dpad_Right.png)    |
| Fire                          | ![](images/RetroPad/Retro_A_Round.png)       |
| Show/Hide Map                 | ![](images/RetroPad/Retro_X_Round.png)       |
| Previous Weapon               | ![](images/RetroPad/Retro_L1.png)            |
| Next Weapon                   | ![](images/RetroPad/Retro_R1.png)            |

## Compatibility

Awaiting description.

## External Links

- [Libretro NXEngine Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/nxengine_libretro.info)
- [Libretro NXEngine Github Repository](https://github.com/libretro/nxengine-libretro)
- [Report Libretro NXEngine Core Issues Here](https://github.com/libretro/nxengine-libretro/issues)
- [Official NXEngine Website](http://nxengine.sourceforge.net/)
- [Official NXEngine Github Repository](https://github.com/EXL/NXEngine)