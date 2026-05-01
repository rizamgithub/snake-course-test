# Gemini Project Instructions - Python Snake Game

This document provides context and instructions for AI agents working on the Python Snake Game project.

## Project Overview
A simple, classic Snake game implemented in Python using the built-in `turtle` graphics module. The project is designed to be lightweight and portable, requiring no external dependencies.

- **Technology Stack:** Python 3 (Standard Library)
- **Graphics Library:** `turtle`
- **Main Entry Point:** `snake.py`

## Architecture and Design
The game follows a functional approach with a main game loop that handles:
1.  **Input Processing:** Responds to arrow keys and WASD for movement.
2.  **Game Logic:** Manages snake movement, growth, food spawning, and collision detection (walls and self).
3.  **Rendering:** Uses `turtle.Screen().update()` with `tracer(0)` for flickering-free animation.

## Building and Running
As this project uses only the Python standard library, there is no build step.

- **Run Game:**
  ```bash
  python snake.py
  ```
- **Dependencies:** None. (Note: `requirements.txt` may exist but is currently empty or contains unused libraries like `pygame` due to environment-specific fallbacks).

## Development Conventions
- **Code Style:** Procedural/Functional. Favor simplicity and readability.
- **Screen Coordinate System:** The game uses an 800x600 window with (0,0) at the center. Boundary collisions occur at +/- 390 units for width and +/- 290 units for height.
- **State Management:** Game state (segments, score, direction) is managed via global variables and object attributes on turtle instances.
- **Naming:** Follow standard PEP 8 conventions where possible.

## Key Files
- `snake.py`: Contains all game logic, rendering, and input handling.
- `README.md`: User-facing documentation.
- `requirements.txt`: Project dependencies (currently unused).
