<h3 align="center">STOP WAR IN 🌻UKRAINE🌻!</h3>
<p align="center">
  <img src="https://github.com/gitendo/gitendo/blob/d91a0a18f414a008c908549328c0f9259bffb399/Russia_Terrorist_Country_480p.gif">
</p>
<h3 align="center">#FCKPTN</h3>

# Hello Game Boy!
This repo started as simple "Hello world!" for Gameboy (DMG) written in assembly language. Few stars later I thought I could start adding some other examples as well, including Game Boy Color (CGB). So here it is - new folder structure, makefiles for Windows / Linux and content that will gradually follow. Everything commented and ready to assemble and link with [RGBASM](https://github.com/rednex/rgbds). Currently it contains:

```
[DMG]
- Hello world
- Display picture composed of 242 unique tiles
- Display picture composed of 355 unique tiles
- Background scroll (clockwise)
- Reading joypad state
- Window
- Single, d-pad moveable sprite
- Meta sprite
- 8x8 sprite collision detection
- Game score in Binary Coded Decimal
- Game score in hexadecimal
- ClockBoy - timer based clock

[CGB]
- Display picture composed of 247 unique tiles, 8 palettes
```
On Windows make sure RGBDS binaries are added to path - here's [how to](https://www.computerhope.com/issues/ch000549.htm) in case you don't know. Otherwise you'd need to change path to files being included and use these commands for each source file:

```
rgbasm.exe -o hello.o hello.s
rgblink.exe -d -o hello.gb hello.o
rgbfix.exe -p 0 -r 0 -v hello.gb 
```
