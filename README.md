# Galaxian Clone

A modern C++ recreation of the classic arcade game **Galaxian**, built using **SDL2** and **SDL2_gfx**.  
This project demonstrates sprite rendering, sound playback, animation, collision handling, and state-based game flow.

---

## Features

- Player ship movement and shooting
- Enemy movement patterns
- Sprite rendering with SDL2
- Background starfield animation
- Sound effects and game loop music
- Menu system
- Modular component-based code structure

---

## Project Structure

The structure below reflects the current repository layout:

```
Galaxian/
├── a.out
├── CON
├── fonts/
│   ├── FreeMono.ttf
│   ├── FreeMonoBold.ttf
│   ├── FreeMonoOblique.ttf
│   ├── FreeMonoBoldOblique.ttf
│   ├── FreeSans.ttf
│   ├── FreeSansBold.ttf
│   ├── FreeSansOblique.ttf
│   ├── FreeSansBoldOblique.ttf
│   ├── FreeSerif.ttf
│   ├── FreeSerifBold.ttf
│   ├── FreeSerifItalic.ttf
│   └── FreeSerifBoldItalic.ttf
│
├── images/
│   └── galaxian/
│
├── includes/
│   ├── Color.h
│   ├── Color.h~
│   ├── compgeom.h
│   ├── Constants.h
│   ├── Event.h
│   ├── Font.h
│   ├── Font.h~
│   ├── Image.h
│   ├── Image.h~
│   ├── Includes.h
│   ├── main.cpp
│   ├── Menu.h
│   ├── Rect.h
│   ├── Rect.h~
│   ├── SDL_gfxPrimitives.h
│   ├── SDL_gfxPrimitives_font.h
│   ├── SingletonSurface.h
│   ├── Sound.h
│   ├── Star.h
│   ├── StarField.h
│   ├── Surface.h
│   ├── Surface.h~
│   ├── TextSurface.h
│   └── TextSurface.h~
│
├── main.cpp
├── main.cpp~
├── main.pdf
├── makefile
├── makefile~
│
├── sounds/
│   ├── explosion.wav
│   ├── GameLoop.ogg
│   └── laser.wav
│
└── src/
    ├── Image.cpp
    ├── Menu.cpp
    ├── SDL_gfxPrimitives.c
    ├── SingletonSurface.cpp
    ├── StarField.cpp
    ├── Surface.cpp
    └── Surface.cpp~
```

---

## Build Instructions

### Requirements

Install SDL2 and SDL2_gfx:

#### Fedora / RHEL
```bash
sudo dnf install SDL2 SDL2-devel SDL2_gfx SDL2_gfx-devel SDL2_mixer SDL2_mixer-devel
```

#### Ubuntu / Debian
```bash
sudo apt install libsdl2-dev libsdl2-mixer-dev libsdl2-gfx-dev
```

---

### Compile

In the project root:

```bash
make
```

Or manually:

```bash
g++ main.cpp src/*.cpp -Iincludes -lSDL2 -lSDL2_mixer -lSDL2_gfx -o galaxian
```

---

## Run the Game

```bash
./galaxian
```

---

## Controls

| Action | Key |
|--------|------|
| Move Left | Left Arrow |
| Move Right | Right Arrow |
| Shoot | Spacebar |
| Quit | Escape |

---

## License

This project is for educational and recreational use.
