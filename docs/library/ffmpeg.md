# FFmpeg

## Background

Video/music player implemented in libretro.

### Author(s):

Fabrice Bellard|FFmpeg team

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/ffmpeg.md). Changes are proposed using "Pull Requests."

## See also

[Imageviewer](https://docs.libretro.com/library/imageviewer/)

[Game Music Emu](https://docs.libretro.com/library/game_music_emu/)

[PocketCDG](https://docs.libretro.com/library/pocketcdg/)

## License

LGPLv2, GPLv2

## Extensions

*Content that can be loaded by the FFmpeg core have the following file extensions.*

mkv|avi|f4v|f4f|3gp|ogm|flv|mp4|mp3|flac|ogg|m4a|webm|3g2|mov|wmv|mpg|mpeg|
vob|asf|divx|m2p|m2ts|ps|ts|mxf|wma|wav

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
| Remapping         | ✔         |
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |

The FFmpeg core's directory name is 'FFmpeg'

## Core options

*The FFmpeg core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.*

- **Temporal Interpolation** (Off/**On**): 'Fake’ a higher framerate by using motion blur.
- **FFT Resolution** (**1280x720**/1920x1080/2560x1440/3840x2160/640x360/320x180): Modify the resolution of the music visualizer.

??? note "FFT Resolution - 320x180"
	![320x180](images\Cores\ffmpeg\320x180.png)
	
??? note "FFT Resolution - 3840x2160"
	![3840x2160](images\Cores\ffmpeg\3840x2160.png)	

- **FFT Multisample** (**1x**/2x/4x): Modify the antialiasing of the music visualizer.
- **Colorspace** (**auto**/BT.709/BT.601/FCC/SMPTE240M): Choose [colorspaces](https://trac.ffmpeg.org/wiki/colorspace) from different broadcast regions/standards.

## Controllers

*The FFmpeg core supports the following controller setting(s), bolded controller settings are the default for the specified user(s):*

### User 1 - 16 Device Type(s)

* **RetroPad** - Joypad with analog

* RetroPad w/Analog - **There is no reason to switch to this.**

### Controllers graph

| FFmpeg               | RetroPad                                                       |
|----------------------|----------------------------------------------------------------|
| Seek +60 seconds     | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Up.png)            |
| Seek -60 seconds     | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Down.png)          |
| Seek -10 seconds     | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Left.png)          |
| Seek +10 seconds     | ![RetroPad_Dpad](images/RetroPad/Retro_Dpad_Right.png)         |
| Cycle Audio Track    | ![RetroPad_L1](images/RetroPad/Retro_L1.png)                   |
| Cycle Subtitle Track | ![RetroPad_R1](images/RetroPad/Retro_R1.png)                   |

## External Links

* [Libretro Repository](https://github.com/libretro/FFmpeg)
* [Report Core Issues Here](https://github.com/libretro/libretro-meta)
* [Official Website](https://www.ffmpeg.org/)
* [Official Repository](https://www.ffmpeg.org/download.html#repositories)