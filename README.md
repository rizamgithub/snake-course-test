# Python Snake Game

A classic Snake game built with Python's standard `turtle` graphics module.

## Project Overview

The game opens an 800x600 window where the player controls a snake, eats food, grows longer, and avoids collisions with the wall or its own body. The score and high score are shown at the top of the game window.

## Requirements

- Python 3.x
- No external packages are required by the current implementation.

> Note: `requirements.txt` currently contains `pygame`, but `snake.py` uses `turtle` from the Python standard library.

## Run

From this folder, start the game with:

```bash
python snake.py
```

## Controls

- `Up`, `Down`, `Left`, `Right`: Move the snake
- `W`, `A`, `S`, `D`: Alternative movement controls

## Gameplay

- Eat the red food to grow the snake.
- Each food item adds 10 points.
- The snake gets slightly faster after eating food.
- Hitting a wall or the snake's body resets the current score and snake length.
- The high score is kept during the current game session.

## Files

- `snake.py`: Main game source code.
- `README.md`: User-facing project documentation.
- `GEMINI.md`: Existing AI-agent context for the project.
- `AGENTS.md`: Agent-facing development notes.
- `requirements.txt`: Currently lists an unused `pygame` dependency.
