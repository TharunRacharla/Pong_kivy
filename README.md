# Pong Kivy

A simple Pong game built with [Kivy](https://kivy.org/). This project follows the official Kivy Pong tutorial and turns it into a small, playable desktop app.

## Features

- Two-player Pong gameplay
- Keyboard-free controls using touch or mouse drag
- Score tracking for both players
- Simple Kivy-based UI and game loop

## Requirements

- Python 3.x
- Kivy and the packages listed in `requirements.txt`

## Installation

1. Clone or download this repository.
2. Open a terminal in the project folder.
3. Install the dependencies:

```bash
pip install -r requirements.txt
```

## Run the game

Start the app with:

```bash
python main.py
```

## How to play

- Move the left paddle by dragging on the left third of the window.
- Move the right paddle by dragging on the right third of the window.
- Keep the ball in play and score when the opponent misses.

## Project structure

- `main.py` contains the game logic, physics, scoring, and app bootstrap.
- `pong.kv` defines the Kivy UI, paddles, ball, and score labels.
- `requirements.txt` lists the Python dependencies needed to run the project.

## How it works

- The game loop runs at 60 FPS using `Clock.schedule_interval`.
- The ball moves using Kivy vector math.
- When the ball collides with a paddle, its direction and speed change.
- When the ball leaves the screen on either side, the opposite player earns a point and the ball is served again from the center.

## Credits

This project is based on the official Kivy Pong tutorial:

https://kivy.org/doc/stable/tutorials/pong.html

## License

No license has been specified yet. Add one if you plan to share or distribute the project.

