# Sega Master System (Emux)

## Background

Emux is a cross-platform emulator project with a goal of emulating multiple kinds of machines related to gaming, such as consoles or arcades. Its philosophy is very much inspired by the Linux kernel (hence the name), which brilliantly manages to support multiple machines while keeping drivers entirely platform-independent. Emux is designed in the same way, keeping a code base of CPUs and controllers separate from machines.

### Why use this core?

-

### Author(s):

Sebastien Ronsse

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/emux_sms.md). Changes are proposed using "Pull Requests."

## See also

[Sega MS/GG/MD/CD (Genesis Plus GX)](https://docs.libretro.com/library/genesis_plus_gx/)

[Sega MS/MD/CD/32X (PicoDrive)](https://docs.libretro.com/library/picodrive/)

## License

GPLv2

## Extensions

*Content that can be loaded by the Emux SMS core have the following file extensions.*

sms|bin|rom

## Database(s)

*RetroArch database(s) that are associated with the Emux SMS core*

* Sega - Master System - Mark III

## BIOS

|   Filename    |    Description                |              md5sum              |
|:-------------:|:-----------------------------:|:--------------------------------:|
| bios.sms      | Master System BIOS - Required | 840481177270d5642a14ca71ee72844c |

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | -         |
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
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |

The Emux SMS core's directory name is 'emux (sms)'

## Controllers

*The Emux SMS core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):*

### User 1 - 16 Device Type(s)

* **RetroPad** - Joypad

* RetroPad w/Analog - Joypad - **There is no reason to switch to this.**

### Controllers graph

| Emux SMS    | RetroPad                                                       |
|-------------|----------------------------------------------------------------|
| 1           | ![RetroPad_B](images/RetroPad/Retro_B_Round.png)               |
| Pause       | ![RetroPad_Start](images/RetroPad/Retro_Start.png)             |
| D-Pad Up    | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            |
| D-Pad Down  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          |
| D-Pad Left  | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          |
| D-Pad Right | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         |
| 2           | ![RetroPad_A](images/RetroPad/Retro_A_Round.png)               |

## Compatibility

Unknown

## External Links

* [Libretro Repository](https://github.com/libretro/emux)
* [Report Core Issues Here](https://github.com/libretro/libretro-meta)
* [Official Website](https://github.com/sronsse/emux)