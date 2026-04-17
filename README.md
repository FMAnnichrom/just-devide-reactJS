# 🐱 Just Divide: Cat Puzzle

A lightweight, fully responsive arithmetic and logic puzzle game built entirely in a single HTML file using **React** and **Tailwind CSS**.

---

## 🎮 Core Mechanic

The core idea is simple: divide strategically to clear the board and create massive combos.

- **Interaction**: Place number tiles next to others to trigger interactions.
- **Merge**: If two tiles are equal, they combine and increase your score.
- **Divide**: If one number can divide the other evenly, a mathematical reduction occurs.
- **Domino Effect**: Smart placements create cascading chain reactions and drastically boost your score multiplier!

---

## 🕹️ How to Play

### 1. Choose Your Difficulty
Select **Easy**, **Medium**, or **Hard**. Each level dynamically scales the pool of numbers and overall spawn complexity.

### 2. Divide and Conquer
Drag tiles from your active queue onto the main grid. Adjacent tiles will:
- **Merge** if identical.
- **Divide** if mathematically valid.

### 3. Tactical Slots
- **[KEEP Slot]**: Save a valuable block for later use and seamlessly swap it back into your active queue strategically.
- **[TRASH Bin]**: Discard unwanted tiles (features limited uses per level, so use them wisely or level-up to earn more).

### 4. Chain Combos
Plan moves to trigger multiple reactions in sequence for the highest possible point bursts!

---

## 🖼️ Assets & Design

* **AI Graphics**: The signature cat graphic character (`assets/cat.png`) was meticulously recreated using AI generation.
* **Layout Mechanics**: The image backgrounds were deliberately trimmed using AI tools to integrate natively into the game UI, perfectly allowing the cat's graphics to visually interact with the board layers (its paws smoothly overlapping the top score edges!).
* **UI/UX Aesthetics**: Features dynamic glassy gradients, bouncing CSS keyframe animations, and custom hybrid-responsive grids to effortlessly switch between compact mobile sizes and widescreen displays.

---

## 💻 Technology Stack

* **Frontend Framework**: React 18 (No cumbersome build tools required, loaded natively via CDN + Babel)
* **Styling**: Tailwind CSS (Loaded via CDN)
* **Logic Environment**: Vanilla ES6 JavaScript directly executed in the browser engine.

---

## 🚀 Running the Game

**Zero setup is required.**

Simply open the `index.html` file natively in any modern web browser to play, or run it through a standard basic local server (e.g., `python -m http.server 3000`).

---

## 🧠 Notes for Developers

The entire game architecture is efficiently organized and deliberately contained within a single `index.html` file to ensure supreme portability and maintainability.

Core mechanic logic is handled directly in JS functions:
- `resolveMerges()` → Handles the complex recursive division and merging reduction chains.
- `processDropOnGrid()` → Oversees player drag-and-drop pointer tile placement and grid validity.
- Core Application State is managed securely using native React hooks (`useState`, `useEffect`).
