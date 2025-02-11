# 🍽️ Food Heuristic in the Game of Pacman

## 📌 Overview
This project implements a **food heuristic** for the classic Pacman game 🕹️ using intelligent search algorithms. The heuristic optimizes Pacman’s movements to efficiently collect food pellets while avoiding unnecessary detours. By incorporating advanced search techniques, this implementation aims to enhance Pacman’s decision-making and improve overall gameplay performance.

## 🌟 Features
✅ Intelligent **food heuristic** to optimize Pacman’s path.  
✅ Uses **A* search, Greedy Best-First Search**, and other search algorithms for better pathfinding.  
✅ Pacman navigates the maze considering the **remaining food pellets** efficiently.  
✅ Built on top of **UC Berkeley’s Pacman AI projects**, adding new enhancements.  

## ⚙️ Installation
Follow these simple steps to get started:

1. **Clone this repository** 📥:
   ```bash
   git clone https://github.com/Arpan-shrma/Food-Heuristic-in-game-of-Pacman.git
   cd Food-Heuristic-in-game-of-Pacman
   ```
2. Ensure you have **Python 3.x** installed 🐍.
3. Install dependencies (if required):
   ```bash
   pip install -r requirements.txt
   ```

## 🎮 Running the Game
To play Pacman with the **food heuristic**, run:
```bash
python pacman.py -l mediumSearch -p SearchAgent -a fn=astar,heuristic=foodHeuristic
```

### 🔹 Example Commands
- Run with **A* Search and Food Heuristic**:
  ```bash
  python pacman.py -l bigSearch -p SearchAgent -a fn=astar,heuristic=foodHeuristic
  ```
- Run with **Greedy Best-First Search**:
  ```bash
  python pacman.py -l smallSearch -p SearchAgent -a fn=gbfs,heuristic=foodHeuristic
  ```

## 🧠 Understanding the Food Heuristic
The heuristic estimates the **optimal path** to collect all remaining food pellets as efficiently as possible. Different approaches include:

🔹 **Manhattan Distance Heuristic**: Measures the distance from Pacman to the closest food pellet.  
🔹 **Minimum Spanning Tree (MST) Heuristic**: Computes the MST of all food locations to estimate the shortest route.  
🔹 **Max Distance Heuristic**: Takes the distance to the farthest food pellet as an estimate of the cost.  

🎯 The goal is to ensure **Pacman follows the most efficient path** while reducing unnecessary moves and avoiding costly detours.  

## 📂 File Structure
📜 `pacman.py` - Main game logic.  
📜 `game.py` - Core engine and game mechanics.  
📜 `search.py` - Implementation of search algorithms.  
📜 `searchAgents.py` - Custom search-based agents.  
📜 `README.md` - Project documentation (this file 📄).  

## 🚀 Future Enhancements
🔹 Implement **machine learning-based heuristics** for dynamic decision-making.  
🔹 Improve performance for **large and complex maps**.  
🔹 Add **visualizations** to track heuristic performance in real-time.  

## 📜 License
This project is **open-source** and available under the **MIT License** 📃.

## 📬 Contact
💡 Have suggestions or want to contribute? Open an **issue** or **pull request** on the repository!  

---
Enjoy playing Pacman with an optimized food heuristic! 🕹️👾

