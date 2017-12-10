# Cave Story (NXEngine)

ScummVM is an interpreter for point-and-click adventure games that can be used as a libretro core.

## Background

[ScummVM](http://scummvm.org) is a program which allows you to run certain classic graphical point-and-click adventure games, provided you already have their data files. The clever part about this: ScummVM just replaces the executables shipped with the games, allowing you to play them on systems for which they were never designed!

### Author(s)

[ScummVM Team](http://www.scummvm.org/credits/)

## Contribute to this documentation

In order to propose improvements to this document, [visit it's corresponding source page on github](https://github.com/libretro/docs/tree/master/docs/library/scummvm.md). Changes are proposed using "Pull Requests."

## License

GPLv2

## Extensions

- .scummvm

## Database(s)

*RetroArch database(s) that are associated with the ScummVM core*

* [ScummVM.dat](https://github.com/libretro/libretro-database/blob/master/dat/ScummVM.dat)

## Features

| Feature           | Supported |
|-------------------|:---------:|
| Saves             | ✔         |
| States            | ✕         |
| Rewind            | ✕         |
| Netplay           | ✕         |
| RetroAchievements | ✕         |
| RetroArch Cheats  | ✕         |
| Native Cheats     | ✕         |
| Controllers       | ✕         |
| Remapping         | ✕         |
| Multi-Mouse       | ✕         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |

### Installation

1. Start up RetroArch. Inside the main menu, go to 'Online Updater'.

2. Just to make sure we have the latest info files, select 'Update Core Info Files'. Wait until this is done. Then, select 'Core Updater'.

3. Browse through the list and select 'ScummVM'.

4. Launch ScummVM by using: Main Menu > Load Core > ScummVM

### Scanning Support

To allow launching ScummVM games from the menu, you'll need to do the following:

1. Look up the Game ID of the game you're looking to add to the menu. Game IDs can be found in [ScummVM's compatibility list](http://scummvm.org/compatibility).
    > `monkey` for Monkey Island

2. Inside the game directory, create a `.scummvm` file, named by the Game ID
    > `monkey.scummvm` for Monkey Island

3. Open up the file in a text editor, and enter in the Game ID.
    > `echo monkey >> monkey.scummvm`

4. (Optional) Alternatively, you could download a prepared `.scummvm` file from [libretro-database-scummvm](https://github.com/RobLoach/libretro-database-scummvm/tree/master/games).

5. Scan each game directory

This is an example of what the playlist would look like:

    /storage/roms/scummvm/monkey/monkey.scummvm
    The Secret of Monkey Island
    /tmp/cores/scummvm_libretro.so
    ScummVM
    b0e2af30|crc
    ScummVM.lpl

## External Links

* [Libretro Repository](https://github.com/libretro/scummvm)
* [Report Core Issues Here](https://github.com/libretro/scummvm/issues)
* [Official Website](http://scummvm.org/)
* [Official Repository](https://github.com/scummvm/scummvm)