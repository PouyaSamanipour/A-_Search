# 🚗 A* Search Algorithm in C++

This project implements the **A\*** pathfinding algorithm in C++. It finds the shortest path between a start and goal location on a grid map with obstacles.

---

## 📖 Overview
- The grid is read from a `.board` file (e.g., `1.board`).
- Each cell can be:
  - `0` → Empty cell
  - `1` → Obstacle
- The algorithm:
  1. Starts at the initial cell (`🚦`)
  2. Expands neighbors using **Manhattan distance** as the heuristic
  3. Continues until reaching the goal cell (`🏁`)
  4. Marks the final path with `🚗`

---

## 🛠️ Features
- A\* search with `f(n) = g(n) + h(n)`
- Custom enum for cell states:
  - `kEmpty`, `kObstacle`, `kClosed`, `kPath`, `kStart`, `kFinish`
- Visualization of the result directly in the console:
  - ⛰️  → Obstacle  
  - 🚗  → Path  
  - 🚦  → Start  
  - 🏁  → Goal  

---

🚦   🚗   0   0   0   0

⛰️   🚗   ⛰️   ⛰️   ⛰️   0

0   🚗   0   0   0   0

0   🚗   0   ⛰️   ⛰️   0

0   🚗   🚗   🚗   🚗   🏁

