# JS_Assignment
# Rubik's Cube - Manual Rotation & Solver 🧩

This project is a fully functional **Rubik's Cube Solver** built using **pure JavaScript** with an **object-oriented approach**. It demonstrates manual face rotation, scrambling, and solving of a 3x3 Rubik's Cube. The main goal is to visualize the steps and logic behind solving any scrambled cube, making it beginner-friendly yet logically sound.

## 🛠 Features

- ✅ Manual rotation of all six faces (U, D, F, B, L, R)
- 🔀 Scramble functionality for random rotations
- ♻️ Reset button to return to default solved state
- 🧠 Solve button that reverses the scramble steps
- 📈 Step-by-step logging of all cube operations
- 🧱 Graphical representation of the cube state at every step
- 📚 Full history pane with previous states in SVG-like text format

## 📐 Technologies Used

- **HTML5** – For page structure and layout
- **CSS3** – For minimal and clean UI
- **Vanilla JavaScript** – No frameworks, 100% custom logic
- **Emoji-based cube rendering** – Visual representation of each colored face
- **Custom getCubeSvgString() function** – Converts cube state into SVG-like string format for visualization

## 🧩 Cube Representation

Each face of the cube is represented as an array of 9 emojis (3x3 grid):
- ⚪ → White (U)
- 🔵 → Blue (D)
- 🟢 → Green (F)
- 🔴 → Red (B)
- 🟠 → Orange (L)
- 🟡 → Yellow (R)

## 🧮 Logic Overview

- **Object-Oriented Structure:** Cube data is maintained as an object with 6 keys (one per face).
- **Rotation:** Face rotations affect both the 9 facelets and adjacent edge stickers.
- **Scramble:** Performs 20 random moves to mix the cube.
- **Solver:** Reverses the scramble history step-by-step (not an optimal algorithm but meets the requirement).
- **History Tracking:** Each state change is captured and visualized in a side pane.

## 📸 UI Sections

| Section      | Description |
|--------------|-------------|
| Current State | Displays the cube in emoji + SVG-style |
| Steps         | Logs each move performed (rotate, scramble, solve) |
| History       | Shows all previous visual states after each move |

