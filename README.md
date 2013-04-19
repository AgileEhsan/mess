# MESS
======

### Enquiring

[MESS](http://http://mess.org) is an amazing program that emulate pretty much every home system that ever existed. The only hickup is that it can be a bit complicated to setup and a lot of the helpers softwares gravitating around it are imperfect or incomplete. Many friends always ask me to it up for them and I got tired to maintain these installations. Git version control seemed to be a good way for me to distribute the setup and have my friend update it easily.

### Installing

For once things will be a bit more complicated for MacOS users since the version of MAME running is actually called [SDLMAME](http://rbelmont.mameworld.info/?page_id=163), and in order to run it you need the [SDL](http://www.libsdl.org/) framework installed. This can be achieved easily following this [video tutorial](http://youtu.be/K6xyO-poAZU?t=30s). On **Windows** there is nothing to do.

### Launching

On **MacOS** open your terminal and browse to mac folder inside the mess folder you just got from GitHub and then issue the following command.

```
./mess64 <sytemename> -<mediatype> <gamename>
```

For example if I want to play Super Mario World on Super Nintendo.

```
./mess64 snes -cart smw
```

You will notice that mame will conveniently propose rom name corrections if you type something slightly inexact. I use that all the time. There is a lot of other possibilities running the emulator through command line and you can have a better idea by typing the following.

```
./mess64 -h
```

For **Windows** just go to the "win" folder instead of the "mac" one and always replace `./mess64` by `mess64.exe`.

### Playing

You play with the keyboard but the emulator is also already configurated to work with most of the fantastic [Retro Zone](http://www.retrousb.com) USB adapters. Main keyboard keys for the first player are 1 for start, 5 to insert coin, WASD for movement and GHJBNM for buttons. For the second player it is respectively 2, 6, ARROWS and 456123 from the numpad.

### Roms

An emulator is not worth much without it's roms but unfortunately I cannot provide them as part of that setup for obvious reasons. Therefore you will have to use you imagination to get a hold on these little gems. Once you find them, the only thing you need to do is create the following folder inside you mess folder.

```
roms/roms
roms/soft
```
The roms folder should have all the system bios roms. These are basically you Super Nintendo, Megadrive, Saturn, etc systems. The soft folder is a bit more complicated.
In there you need to have a specific folder for each individual system and put the roms of that specific system in there. Let me give you a little map for the main ones.

* **snes:** Super Nintendo / Super Famicom
* **nes:** Nintendo, Famicom
* **gameboy:** Game Boy
* **saturn:** Saturn
* **pce:** PC Engine
* **psx:** Playstation
* **cpc_flop:** Amstrad Floppies
* **gba:** Game Boy Advance
* **megadriv:** Megadrive / Genesis
* **n64:** Nintendo 64

In order to know more about this and expected rom names you will need to have a look at the hash folder that hold descriptions of supported games for each system. This is not perfect but will improve as MESS evolves.