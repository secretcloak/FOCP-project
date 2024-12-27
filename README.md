# Project Title 
- Space Shooter Clone

## Group Members
- Luqman Shahzad (507599).

## Credits
 Hamza Yaqoob (BE-EE 3rd semester) for function delete bullets and enemies.

## Project Description
"Space Shooter Clone" is a 2D space shooting game where the player controls a spaceship to defeat enemy ships while avoiding collisions. The game is designed with progressive difficulty, including increasing enemy strength, and a scoring system to track player performance. The game ends when the player collides with an enemy or completes the final level (Level 10). The project is implemented using the SFML (Simple and Fast Multimedia Library) framework.

## Features
- **Player Ship**: Move left or right and fire bullets to destroy enemies.
- **Enemies**: Randomly spawn with different movement patterns and speeds that increase with levels.
- **Bullets**: Player fires bullets to eliminate enemies.
- **Scoring System**:
  - +10 points for hitting an enemy.
  - -10 points for letting an enemy pass the screen.
- **Level Progression**:
  - Difficulty increases with each level (up to Level 10).
  - Enemies move faster as the level increases.
- **Win and Game Over Conditions**:
  - Win: Achieve Level 10.
  - Game Over: Collide with an enemy ship.
- **Sound Effects**:
  - Explosions when an enemy is destroyed.
  - Game over and victory soundtracks.
- **Reset Functionality**:
  - Restart the game manually or upon game over/victory.
- **Replay and Exit Controls**:
  - Press `P` to restart.
  - Press `ESC` to exit the game.

## Architecture/Structure

- Main Components:
1. **Player**:
   - Controlled by keyboard inputs (`Left` and `Right` arrows to move, `Space` to shoot).
   - Player's position and movement are restricted within the screen bounds.

2. **Enemies**:
   - Stored in an array and dynamically spawn during gameplay.
   - Each enemy has randomized horizontal and vertical movement speeds.
   - Enemies bounce off screen edges and move down toward the player.

3. **Bullets**:
   - Stored in an array.
   - Fired by the player and move vertically upward.
   - Destroyed upon collision with an enemy or exiting the screen.

4. **Collision Detection**:
   - Bullets and enemies are checked for collisions.
   - Player and enemies are checked for collisions.

5. **Game Logic**:
   - **Level Progression**: Score thresholds determine level-ups.
   - **Score Management**: Incremented or decremented based on player actions.
   - **Reset Functionality**: Resets all variables (score, level, bullets, enemies) to their initial state once       
   -                          the player presses P after Game over or Win. 
6. **Graphics**:
   - Player, enemies, and background are rendered using SFML textures.
   - Text is used to display the score and level.

7. **Audio**:
   - Sound effects for explosions, game over, and victory.

## How to Run and Deploy the Project

### Prerequisites:
1. Install a C++ compiler (e.g., GCC or MSVC).
2. Install SFML (Simple and Fast Multimedia Library):
   - Download from [SFML's official website](https://www.sfml-dev.org/).
   - Follow the installation instructions for your platform.
3. Clone the GitHub repository containing the source code.

### Steps to Run:
1. Clone the repository:
   ```bash
   git clone <your-github-link>
   cd space-shooter-clone
   ```
2. Open the project in your preferred C++ IDE (e.g., Visual Studio, Code::Blocks).
3. Link SFML libraries to your project:
   - `sfml-graphics`
   - `sfml-window`
   - `sfml-system`
   - `sfml-audio`
4. Build and run the project from your IDE.

### How to Play:
1. Use `Left Arrow` and `Right Arrow` keys to move your spaceship.
2. Press `Spacebar` to shoot bullets at enemies.
3. Avoid collisions with enemy ships.
4. Destroy enemies to score points and progress through levels.
5. Pause or restart the game with `P`.
6. Exit the game with `ESC`.

### Folder Structure:
```
Space-Shooter-Clone/
├── Assets/             # Contains textures, sounds, and fonts
├── Main                # Source code file
├── README.txt          # Detailed project documentation
'''
