# NES / Famicom (Emux NES)

## Contribute to this documentation

**In order to propose improvements to this document, [visit its corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/emux_nes.md). Changes are proposed using "Pull Requests."**

**There is a To-Do list for libretro/docs [here](https://docs.libretro.com/docguide/todo/)**

**You can submit suggestions or issues regarding documentation at the [libretro/docs issue tracker](https://github.com/libretro/docs/issues) or in our [forum thread](https://forums.libretro.com/t/wip-adding-pages-to-documentation-site/10078/).**

## Background

Emux is a cross-platform emulator project with a goal of emulating multiple kinds of machines related to gaming, such as consoles or arcades. Its philosophy is very much inspired by the Linux kernel (hence the name), which brilliantly manages to support multiple machines while keeping drivers entirely platform-independent. Emux is designed in the same way, keeping a code base of CPUs and controllers separate from machines.

### Why use this core?

Awaiting description.

### How to get and install the Emux NES core:

- Start up RetroArch. Inside the main menu, go to 'Online Updater'.

<center> ![](images\Cores\all\updater.png) </center>

- Just to make sure we have the latest info files, select 'Update Core Info FIles'. Wait until this is done. Then, select 'Core Updater'.

<center> ![](images\Cores\all\info.png) </center>

- Browse through the list and select 'NES / Famicom (Emux NES)'.

<center> ![](images\Cores\emux\emux_nes.png) </center>

After this has finished downloading, the core should now be ready for use!

#### How to start (after installation):

- Go back to RetroArch's main menu screen. Select 'Load Content'.

<center> ![](images\Cores\all\load.png) </center>

- Browse to the folder that contains the content you want to run.

- Select the content that you want to run.

<center> ![](images\Cores\all\nes.png) </center>

- If you are asked which core to select, choose 'NES / Famicom (Emux NES)'.

The content should now start running!

### Authors

- Sebastien Ronsse

## See also

### NES/Famicom

- [NES / Famicom (bnes)](https://docs.libretro.com/library/bnes/)
- [NES / Famicom (FCEUmm)](https://docs.libretro.com/library/fceumm/)
- [NES / Famicom (Nestopia UE)](https://docs.libretro.com/library/nestopia_ue/)
- [NES / Famicom (QuickNES)](https://docs.libretro.com/library/quicknes/)

## License

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

The Emux NES core is licensed under

- [GPLv2](https://github.com/libretro/emux/blob/master/COPYING)

## Extensions

Content that can be loaded by the Emux NES core have the following file extensions:

- .nes
- .bin
- .rom

## Databases

RetroArch database(s) that are associated with the Emux NES core:

- [Nintendo - Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Nintendo%20Entertainment%20System.rdb)

## Features

RetroArch-level settings or features that the Emux NES core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✕         |
| States            | ✕         |
| Rewind            | ✕         |
| Netplay           | ✕         |
| Core Options      | ✕         |
| RetroAchievements | ✕         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✕         |
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

The Emux NES core's directory name is 'emux (nes)'

### Geometry and timing

- The Emux NES core's internal FPS is (FPS)
- The Emux NES core's internal sample rate is (Rate)
- The Emux NES core's core provided aspect ratio is (Ratio)

## Controllers

### Device types

The Emux NES core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

#### User 1 - 2 device types

- None - Doesn't disable input.
- **RetroPad** - Joypad
- RetroPad w/Analog - Joypad - There is no reason to switch to this.

### Controller tables

#### Joypad and analog device type table

| User 1 - 2 Input descriptors  | RetroPad Inputs                              | RetroPad           |
|-------------------------------|----------------------------------------------|--------------------|
|                               | ![](images/RetroPad/Retro_B_Round.png)       | B                  |
|                               | ![](images/RetroPad/Retro_Select.png)        | Select             |
|                               | ![](images/RetroPad/Retro_Start.png)         | Start              |
|                               | ![](images/RetroPad/Retro_Dpad_Up.png)       | D-Pad Up           |
|                               | ![](images/RetroPad/Retro_Dpad_Down.png)     | D-Pad Down         |
|                               | ![](images/RetroPad/Retro_Dpad_Left.png)     | D-Pad Left         |
|                               | ![](images/RetroPad/Retro_Dpad_Right.png)    | D-Pad Right        |
|                               | ![](images/RetroPad/Retro_A_Round.png)       | A                  |

## Compatibility

Awaiting description.

## External Links

- [Libretro Emux GB Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/emux_gb_libretro.info)
- [Libretro Emux GB Github Repository](https://github.com/libretro/emux)
- [Report Libretro Emux GB Core Issues Here](https://github.com/libretro/libretro-meta/issues)
- [Official Emux GB Github Repository](https://github.com/sronsse/emux)