# Py-runner

An endless runner game built with Pygame. A player character jumps over randomly spawned obstacles — snails on the ground and flies in the air — while the score climbs with survival time.

## Gameplay

- Obstacles spawn randomly: ground snails and airborne flies
- Score increases each frame you survive
- Background music plays throughout; a jump sound fires on each jump
- The game restarts automatically on collision

## Controls

| Key | Action |
|:---|:---|
| `SPACE` | Jump / start the game |
| Close window | Quit |

## Requirements

- Python 3.8+
- `pygame-ce`

```bash
pip install pygame-ce
```

## Run

```bash
python "runner_class only.py"
```

## Project Structure

```
Py-runner/
├── runner_class only.py    # Main game entry point
├── player.py               # Player sprite and jump logic
├── obstacle.py             # Fly and snail obstacle classes
├── audio/                  # Background music and sound effects
├── graphics/               # Sprite sheets and background images
└── font/                   # Score display font
```

## How It Works

The game uses a class-based structure with three modules:

- **`player.py`** — handles player animation frames, gravity, and jump state
- **`obstacle.py`** — manages fly and snail sprite selection, random spawn positioning, and movement
- **`runner_class only.py`** — main game loop: event handling, collision detection, score rendering, and group updates
