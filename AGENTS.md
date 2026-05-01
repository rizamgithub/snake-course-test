# Agent Notes - Python Snake Game

## Project Context

This folder contains a simple Python Snake game. The active implementation is in `snake.py` and uses the Python standard library `turtle` module for graphics.

The current game is procedural and keeps game state in module-level variables:

- `delay`: Controls game speed.
- `score` and `high_score`: Track scoring.
- `head`: Turtle object for the snake head.
- `food`: Turtle object for the food.
- `segments`: List of turtle objects for the snake body.
- `pen`: Turtle object for score rendering.

## How to Run

```bash
python snake.py
```

No build step is required.

## Dependencies

The code does not import any third-party packages. `requirements.txt` currently contains `pygame`, but that package is not used by `snake.py`.

## Game Behavior

- Window size: 800x600.
- Movement step: 20 pixels.
- Boundary collision limits: `x > 390`, `x < -390`, `y > 290`, `y < -290`.
- Food spawns randomly within approximately the playable area.
- Eating food adds one body segment, increases score by 10, and reduces delay by `0.001`.
- Wall or self collision resets the snake, score, and delay while preserving high score.
- Supported controls: arrow keys and `W`, `A`, `S`, `D`.

## Development Guidance

- Keep the project lightweight unless the user explicitly asks for a larger framework or dependency.
- Preserve the simple procedural style unless a refactor is part of the request.
- If changing movement or collision logic, check that the 20-pixel grid behavior remains consistent.
- If updating documentation, describe the implementation as `turtle`-based, not `pygame`-based.
- Avoid adding unrelated files or broad refactors for small gameplay changes.
