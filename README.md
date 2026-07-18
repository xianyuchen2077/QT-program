# qt_programming_2024

A two-player 2D battle game developed with **C++ and Qt 6** as a course project.

## Project Goal

The project explores desktop game development with Qt's Graphics View framework. It combines scene management, keyboard input, character movement, combat, equipment, item pickup, and a settings interface in a modular C++ application.

## Core Features

- Two controllable player characters in a 1280 × 720 battle scene
- Ice-field and grassland modes with scene switching and restart support
- Character movement, jumping, crouching, pickup, attack, and collision handling
- Multiple weapon and projectile types, including pistol, solid ball, sniper rifle, fist, and knife
- Armor, head equipment, leg equipment, and medical supplies
- Randomized item drops and mountable equipment
- Settings scene and menu-based scene navigation

## Technical Stack

- C++17
- Qt 6 Core, Gui, and Widgets
- Qt Graphics View (`QGraphicsScene`, `QGraphicsView`, and graphics items)
- Qt signals and slots
- CMake 3.28 or later

## Project Structure

```text
.
├── CMakeLists.txt        # Qt target and source-file configuration
├── assets/               # Images and Qt resource collection
├── src/
│   ├── MyGame.*          # Main window and scene switching
│   ├── Scenes/           # Battle, ice-field, and settings scenes
│   └── Items/            # Characters, maps, weapons, bullets, equipment, and supplies
└── build/                # Existing generated build artifacts
```

## Build and Run

Install a Qt 6 development environment and CMake 3.28 or later, then configure and build the project from the repository root:

```bash
cmake -S . -B build
cmake --build build --config Release
```

If CMake cannot locate Qt, set `CMAKE_PREFIX_PATH` or `Qt6_DIR` to the local Qt installation before configuring. The executable target is `qt_programming_2024`.

## Contribution Scope

The repository's visible history contains one commit authored by `xianyuchen2077`, covering the submitted CMake configuration, source code, and assets. That confirms responsibility for assembling and submitting this repository version.

The Git history does not preserve enough intermediate commits to attribute every class or distinguish any collaboration that may have occurred during the course. **TODO:** document the original team status and module-level division of work if additional course records are available.

## Limitations

- No automated test suite is included in the repository.
- Generated build artifacts are already tracked alongside the source.
- Platform-specific compiler and Qt installation details are not documented in the original project history.
- **TODO:** add verified gameplay controls and screenshots from a tested build.
