# 3D Look Snake Game with Detailed Rats and Hedgehogs

## Overview

This project is a modern take on the classic Snake game, featuring 3D-looking snakes, detailed rats, and hedgehogs. The game includes additional features such as blood splatter effects, collision detection with walls, and sound effects for various events. The game is developed using Pygame.

## Features

- **3D Look Snake**: The snake is rendered with realistic shadows, eyes, and fangs to give a 3D appearance.
- **Detailed Rats**: Rats randomly emerge from the edges of the walls, can eat the apple, and have shadows, eyes, ears, teeth, and tails. When the snake eats a rat, the rat makes a squeak sound, and blood splatter is generated.
- **Hedgehogs**: Hedgehogs also emerge from the edges of the walls, and when eaten by the snake, they cause the snake to blink in red and green, slow down for 5 seconds, and generate blood splatter.
- **Realistic Shadows and Lighting**: Objects like the snake, rats, hedgehogs, and apples have realistic shadows.
- **Sound Effects**: Various sound effects for eating apples, rats, crashing into walls, and warnings when eating hedgehogs.
- **Blood Splatter Effects**: Blood splatters are generated when the snake eats a rat or hedgehog, or crashes into a wall.
- **Collision Detection**: The snake dies when it collides with the wall or itself, with appropriate sound effects and visual feedback.

## Directory Structure

```
snake_game/
├── assets/
│   ├── sounds/
│   │   ├── crunch.mp3
│   │   ├── rat_squish.mp3
│   │   ├── snake_squish.mp3
│   │   ├── rat_squeak.mp3
│   │   ├── hedgehog_squeak.mp3
│   │   └── snake_crunch.mp3
│   └── images/
│       └── wood_texture.png
├── src/
│   ├── __init__.py
│   ├── config.py
│   ├── game.py
│   ├── snake.py
│   ├── rat.py
│   ├── hedgehog.py
│   └── utils.py
└── README.md
```

## Installation

1. **Clone the repository:**

   ```sh
   git clone https://github.com/showman-sharma/snake_plus.git
   cd snake_game
   ```

2. **Install the required dependencies:**

   ```sh
   pip install pygame
   ```

3. **Ensure the assets are in the correct directories:**

   - Place all sound files (`crunch.mp3`, `rat_squish.mp3`, `snake_squish.mp3`, `rat_squeak.mp3`, `hedgehog_squeak.mp3`, and `snake_crunch.mp3`) in the `assets/sounds/` directory.
   - Place the wood texture image (`wood_texture.png`) in the `assets/images/` directory.

## How to Play

1. **Run the game:**

   ```sh
   python src/game.py
   ```

2. **Controls:**
   - Use the arrow keys to move the snake.
   - The objective is to eat the apples to grow the snake.
   - Avoid running into the walls or the snake itself.

3. **Additional Game Mechanics:**
   - **Rats**: Rats appear randomly and can eat the apple. If the snake eats a rat, the rat makes a squeak sound, and blood splatter is generated.
   - **Hedgehogs**: Hedgehogs appear randomly, and when eaten by the snake, they cause the snake to blink in red and green, slow down for 5 seconds, and generate blood splatter.
   - **Blood Splatter**: Blood splatters are generated when the snake eats a rat or hedgehog, or crashes into a wall.
   - **Game Over**: The game ends when the snake collides with the wall or itself. A wooden textured board with a "You Lost!" message is displayed, and you can press `Q` to quit or `C` to play again.

## Code Explanation

### `config.py`

This file contains all the configuration settings, including screen dimensions, colors, game variables, and sound files.

### `utils.py`

This file contains utility functions for drawing the grass, brick fencing, apple, blood splatter, wall holes, and the wooden board.

### `game.py`

This is the main game file. It handles the game loop, event handling, drawing objects on the screen, and playing sound effects.

### `snake.py`

This file contains functions related to the snake, including drawing the snake.

### `rat.py`

This file contains functions for spawning, moving, and drawing rats, as well as playing the appropriate sound effects when a rat is spawned or eaten.

### `hedgehog.py`

This file contains functions for spawning, moving, and drawing hedgehogs, as well as playing the appropriate sound effects when a hedgehog is spawned or eaten.

## Future Improvements

- Add more obstacles and power-ups.
- Implement different game levels with increasing difficulty.
- Add a high score feature.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the Apache 2.0 License.
