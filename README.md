🎮 2048 Game in MATLAB

This is a complete recreation of the popular 2048 game built in MATLAB, featuring a fully functional GUI with mouse and keyboard controls.

🧩 Features

Playable 2048 game with a graphical interface.

Fully supports both keyboard arrow keys and on-screen buttons.

Tracks score and best score, saved between sessions (best.mat).

Implements core 2048 logic including tile merging, random tile generation, and game over detection.

Customizable tile colors and font sizes based on the tile values.

🚀 How to Run

Open MATLAB.

Place the game2048.m file in your working directory.

Run the file:

game2048

Requires no additional toolboxes.

🎮 Controls

Arrow keys: Move tiles (↑ ↓ ← →).

On-screen buttons: Also available for up, down, left, and right movement.

New Game button: Resets the game board and score.

When no moves are left, a Game Over screen is displayed with an option to restart.

📦 Files

game2048.m: The full source code of the game, including GUI and logic.

best.mat: A file that stores the highest score achieved across game sessions (auto-generated on first run).

🛠 Code Structure

Main Game Function: game2048 initializes the UI and contains all nested logic functions.

Subfunctions:

moveevent: Handles the merging and shifting of tiles.

createNewNum: Randomly generates a new tile (2 or 4).

drawSquare: Updates UI elements (tile values, colors, fonts).

judge: Checks for game over conditions.

gameOver: Triggers the end-game UI.

restart: Resets the game state.

init: Initializes the GUI components.

📐 Visual Layout

4×4 grid using uicontrol elements (edit fields).

Buttons and labels for score, best score, game title, and Game Over overlay.

Responsive design for both interaction styles (mouse + keyboard).

🖼 Screenshot (Optional)

(You can insert a screenshot of the game GUI here)


👨‍💻 Author
Developed by Ivan Efimov

