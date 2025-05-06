# 🎮 2048 Game in MATLAB

This is a complete implementation of the classic [2048 game](https://play2048.co/) built entirely in **MATLAB**.  

---

## 🧩 Features

- 🟦 4×4 dynamic grid built with `uicontrol`
- 🎨 Colored tiles and adaptive font sizes
- ⌨️ Keyboard arrow key support (↑ ↓ ← →)
- 🖱 GUI buttons for directional control
- 💾 Persistent **Best Score** saved in `best.mat`
- 🛑 Game over detection and overlay message
- 🔄 "New Game" button for easy restart

---

## 🚀 How to Run

1. Open **MATLAB**.
2. Place the `game2048.m` file in your current working directory.
3. Run the following in the Command Window:
   ```matlab
   game2048

🎮 Controls
You can use either keyboard or GUI buttons for gameplay.

| Input               | Action                 |
| ------------------- | ---------------------- |
| ↑ (Up Arrow)        | Move tiles up          |
| ↓ (Down Arrow)      | Move tiles down        |
| ← (Left Arrow)      | Move tiles left        |
| → (Right Arrow)     | Move tiles right       |
| `New Game` button   | Restart the game       |
| On-screen `▲ ▼ ◀ ▶` | Alternate GUI controls |

Both keyboard and button inputs trigger the same internal logic.

📂 Files Included

| File                     | Description                                   |
| ------------------------ | --------------------------------------------- |
| `game2048.m`             | Main source code (GUI + game logic)           |
| `best.mat`               | Auto-created on first run to store best score |
| `README.md`              | Project description (this file)               |

🧠 Code Structure Overview
🗂 Main Logic (Nested Functions inside game2048.m)

| Function                                      | Description                                          |
| --------------------------------------------- | ---------------------------------------------------- |
| `moveevent`                                   | Handles tile shifting and merging logic (row-wise)   |
| `createNewNum`                                | Randomly inserts a new 2 or 4 into an empty tile     |
| `judge`                                       | Checks if any moves are possible; triggers game over |
| `drawSquare`                                  | Updates tile colors, text, and scores                |
| `gameOver`                                    | Displays "Game Over" UI overlay                      |
| `restart`                                     | Clears and resets the board                          |
| `init`                                        | Initializes all UI components and game state         |
| `key`                                         | Keyboard key binding logic (arrow keys)              |
| `upmove`, `downmove`, `leftmove`, `rightmove` | Button control callbacks                             |

🧱 GUI Elements

All elements are created using uicontrol programmatically:

Grid: 16 editable fields (4×4)

Score & Best: Static text labels

Directional Buttons: Buttons with Unicode arrows

Game Over Overlay: Hidden label + restart button

Restart Button: "New Game" in bottom-right

💾 Best Score Persistence

Automatically saved in a file named best.mat.

Updates after each game session or restart.

Reloaded on every launch to retain progress.

🖼 Screenshot 

![image](https://github.com/user-attachments/assets/b4a9f756-a51b-4735-8bee-15c392b8a6a3)

📄 License
This project is licensed under the MIT License. Feel free to use, modify, and distribute.

👨‍💻 Author

Developed by Ivan Efimov

