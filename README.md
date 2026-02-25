# 2048 ⁂
a 2048 game implementation using SDL2 in C. this project involves creating a simple version of the classic 2048 game, where players slide tiles on a grid to combine them into a tile of 2048.

## features
- **user**: classic gameplay for the player.
- **user vs machine**: play against an AI opponent.
- **user interface**: simple, clean interface with animated tiles.
- **ranking system**: keeps track of the best scores.
- **sound and music**: background music and sound effects.


## screenshots

![Alt text](Screenshots/Welcomepic.png)

---

![Alt text](Screenshots/play.png)


---


![Alt text](Screenshots/PlayerVSMACHINE.png)


## requirements
- **SDL2**: make sure SDL2 is installed on your system. follow the instructions on the official SDL website to install it: [SDL2 Installation](https://wiki.libsdl.org/Installation).
- **SDL2_ttf**: required for rendering text. install it similarly to SDL2.
- **C compiler**: GCC or Clang recommended for compiling the project.

### installing dependencies
to install the dependencies on Linux (for example, Ubuntu), run:
```bash
sudo apt-get install libsdl2-dev libsdl2-ttf-dev
```

and for Arch linux based systems:
```bash
sudo pacman -S sdl2 sdl2_ttf sdl2_image sdl2_mixer
```
```bash
sudo pacman -S ffmpeg
```


## directory structure
```
|-- assets/
|   |-- Letter.ttf              # font file used for rendering text in the game
|   |-- LilitaOne-Regular.ttf   # font file used for rendering text in the game
|   |-- NType82.otf             # font file used for rendering text in the game
|   |-- NType82.ttf             # font file used for rendering text in the game
|   |-- Ndot-55.ttf             # font file used for rendering text in the game
|   |-- OFL.txt                 # font license information
|   |-- assets_watchdogs.mp3    # background music
|   |-- cyberpunk.mp4           # video file for the game intro
|   |-- icon.jpg                # icon used in the game window
|
|-- include/
|   |-- cgame.h                 # contains game logic declarations
|   |-- input.h                 # input handling functions
|   |-- render.h                # rendering functions for drawing the game board and UI
|   |-- utils.h                 # utility functions for randomization and other helper tasks
|
|-- cgame.c                 # core game logic implementation
|-- input.c                 # input handling code
|-- render.c                # rendering logic using SDL
|-- utils.c                 # helper functions and utilities
|-- main.c
|
|-- README.md                  # project documentation
```

## installation and compilation
after installing files, we can complie and make the executable file of the game(noting that the Directory structure need to be respected in order to be able to compile)

we can do this by typing the following command:
```shell
gcc -g -o "NumberSlide.exe" main.c render.c input.c utils.c cgame.c -I include -lSDL2 -lSDL2_ttf -lSDL2_image -lSDL2_mixer -lavcodec -lavformat -lavutil -lswscale -lm
```


## how to play
-  arrow keys: move tiles on the grid.
-  press 'Esc': exit the game.
-  when you exit without finsing your game, you will be asked if you want to resume your last game or start a new one in your next launch of the game


## credits
group project for DSA III class — USTHB 2024
