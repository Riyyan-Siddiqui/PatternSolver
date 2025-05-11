# 🧩 Sliding Puzzle Solver

A sleek and powerful sliding puzzle solver and visualizer — built to help you explore and understand classic search algorithms and an efficient, human-like solving strategy for puzzles of *any size*. Designed for mobile-first use as a **Progressive Web App (PWA)**.

🔗 [What is a sliding puzzle?](https://en.wikipedia.org/wiki/Sliding_puzzle)

---

## 🚀 Features

- ✅ **Solve Any Puzzle Size**  
  Solve NxP sliding puzzles using a **fast, non-optimal strategic algorithm** based on human techniques.

- 📊 **Algorithm Visualizer**  
  Compare runtimes and memory usage of common search algorithms using 3x3 puzzles:
  - **Breadth-First Search (BFS)**
  - **A\* Search** (with and without closed list)
  - **Iterative Deepening A\*** (IDA\*)

- 🧠 **Edit & Experiment Freely**
  - Solve manually using drag and drop
  - Edit start and goal states
  - Shuffle or reset puzzle
  - Rotate or flip tiles
  - Resize puzzle board dynamically
  - Randomize size and tile state

- 🖼️ **Custom Backgrounds**
  - Upload local or URL-based images
  - Flip background image horizontally/vertically
  - Toggle grid borders and tile numbers

- 📱 **Progressive Web App (PWA)**
  - Fully mobile-friendly
  - Installable and offline-capable

---

## 🧩 Strategic Solving Algorithm

This project includes a strategic algorithm to efficiently solve large puzzles. It’s based on [WikiHow’s human method](https://www.wikihow.com/Solve-Slide-Puzzles), adapted for custom goal states and optimized for performance.

### 🔧 Rules & Strategy

```text
1. If the puzzle is non-square, solve rows or columns until the remaining puzzle is square.
2. Alternate solving rows and columns until a 2x2 remains (must include the blank tile).
3. Direction of solving:
   - Solve rows top-down and columns left-right.
   - If on the goal's blank tile row/column, reverse direction.
4. Once a tile is in its goal position, never move it again.
   - Each solved row/column reduces the problem space.
   - Keep blank inside the unsolved inner area.




# Setup
This project has no runtime dependencies.  Mocha and Webpack are included as dev dependencies for testing, minifying assets, and adding a local web server to auto-refresh assets during development 

Install the dev dependencies with:
```
npm install
```

You can run a development server locally that auto-refreshes assets with:
```
npm start
```

Output minified assets for production with:
```
npm run build
```


# Feature list
* Solve any sized NxP sliding puzzle with any start and goal state incredibly fast with custom strategic algorithm
* Visualize and compare runtimes and memory usage common search algorithms for 3x3 sliding puzzles
  * Breadth-first Search
  * A* (with and without closed list/set)
  * IDA* (Iterative Deepening)
* UI utilities
  * Allow user to solve puzzle themselves, following regular sliding rules
  * Edit puzzle goal and start states 
    * Click/drag to swap tiles
    * Allows for all possible start and goal states
  * Resize puzzle
  * Shuffle Puzzle
  * Reset Puzzle
  * Rotate Puzzle
  * Flip puzzle tiles horizontally/vertically
  * Randomize puzzle size and state using above
  * Custom background image
    * Local image upload
    * External image URL upload
  * Flip background image horizontally/vertically
  * Toggle borders on puzzle grid
  * Toggle numbers on puzzle grid
