# Galaxian Clone

A lightweight C++/SDL2 remake of the classic Galaxian arcade shooter.  
Designed with a clean architecture, predictable game-loop timing, and extendable components.

## Features

- Player ship movement and firing
- Enemy formations with swooping attack patterns
- Collision detection for bullets and enemies
- Sprite rendering and basic animations
- Wave progression system
- Configurable FPS locking

## Technology

- C++17+
- SDL2
- CMake
- PNG spritesheets and simple SFX

## Project Structure

```
/src
    main.cpp
    Game.cpp / Game.hpp
    Player.cpp / Player.hpp
    Enemy.cpp / Enemy.hpp
    EnemyFormation.cpp / EnemyFormation.hpp
    Bullet.cpp / Bullet.hpp
    Renderer.cpp / Renderer.hpp
    AssetLoader.cpp / AssetLoader.hpp
/assets
    sprites/
    sounds/
/build
CMakeLists.txt
README.md
```

## Build Instructions

### Prerequisites
- C++17 compatible compiler
- SDL2 development libraries
- CMake 3.10+

### Steps
```bash
mkdir build
cd build
cmake ..
make
```

### Run
```bash
./galaxian
```

## Controls

| Action       | Key                |
|--------------|--------------------|
| Move Left    | Left Arrow / A     |
| Move Right   | Right Arrow / D    |
| Fire         | Space              |
| Quit         | Esc                |

## Known Limitations

- Enemy AI simplified vs. original arcade implementation
- Basic sound handling

## Roadmap

- High score saving
- Menu + settings UI
- More accurate enemy behavior
- Explosion animations and particles
- WebAssembly or SDL3 port

