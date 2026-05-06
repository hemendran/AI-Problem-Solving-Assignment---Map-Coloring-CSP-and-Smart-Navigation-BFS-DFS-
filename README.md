# AI Problem Solving — RA2411026050336

> **Artificial Intelligence — Problem Solving Assignment**  
> GitHub Submission | Interactive Web-Based Solutions

---

## 👤 Team Details

| Field | Details |
|-------|---------|
| Register Number | RA2411026050336 |
| Repository | AI_ProblemSolving_RA2411026050336 |

---

## 📁 Repository Structure

```
AI_ProblemSolving_RA2411026050336/
│
├── Problem5_MapColoring/
│   └── map_coloring.html        ← Interactive Map Coloring (CSP)
│
├── Problem8_SmartNavigation/
│   └── smart_navigation.html    ← Smart Navigation System (BFS + DFS)
│
└── README.md
```

---

## 🧩 Problem 5 — Map Coloring Problem (CSP)

### Problem Description
Color regions of a map such that no two adjacent regions share the same color, using the minimum number of colors possible.

### Algorithm Used
- **Constraint Satisfaction Problem (CSP)**
- **Backtracking Search** with forward checking
- Dynamic constraint propagation

### How to Run
1. Open `Problem5_MapColoring/map_coloring.html` in any browser
2. Enter region names (comma separated)
3. Enter adjacency pairs (e.g., `A-B`)
4. Choose available colors
5. Click **SOLVE WITH CSP**

### Features
- Interactive graph visualization (SVG)
- Real-time backtracking trace log
- Color chips displayed per region
- India Map preset example
- Stats: regions, colors used, backtracks

### Sample Input
```
Regions: A, B, C, D
Adjacency: A-B, A-C, B-C, B-D, C-D
Colors: Red, Green, Blue
```

### Sample Output
```
A → Red
B → Green
C → Blue
D → Red
✓ SOLVED | Backtracks: 0
```

---

## 🗺️ Problem 8 — Smart Navigation System (BFS & DFS)

### Problem Description
Find a route between two locations in a city graph. Compare BFS (guarantees shortest path) and DFS (memory efficient, faster in some cases).

### Algorithms Used
- **Breadth-First Search (BFS)** — explores level by level, guarantees shortest path
- **Depth-First Search (DFS)** — explores deeply first, not always shortest

### How to Run
1. Open `Problem8_SmartNavigation/smart_navigation.html` in any browser
2. Enter node names (comma separated)
3. Enter edges (e.g., `A-B`)
4. Set Start Node and Goal Node
5. Click **RUN BFS + DFS**

### Features
- Canvas-based animated graph drawing
- Side-by-side BFS vs DFS path comparison
- Detailed comparison table (path length, nodes explored, optimality)
- Color-coded: Blue = BFS path, Yellow = DFS path, Green = Start/Goal

### Sample Input
```
Nodes: A, B, C, D, E, F, G
Edges: A-B, A-C, B-D, B-E, C-F, D-G, E-G, F-G
Start: A   Goal: G
```

### Sample Output
```
BFS Path: A → B → D → G  (length: 3, optimal ✓)
DFS Path: A → B → D → G  (length: 3)
Nodes explored — BFS: 5  |  DFS: 4
```

---

## 📊 Comparison Summary

| Feature | BFS | DFS |
|---------|-----|-----|
| Guarantees Shortest Path | ✅ Yes | ❌ No |
| Space Complexity | O(V) — wide | O(depth) — lean |
| Best For | Shortest path | Memory saving |
| Explores | Level by level | Deep first |

---

## ▶️ Execution Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/AI_ProblemSolving_RA2411026050336.git
   ```
2. Navigate to any problem folder
3. Open the `.html` file directly in a browser — **no server or installation needed**
4. Interact with the UI to test different inputs

---

## 🛠️ Tech Stack

- **Language:** HTML5 + CSS3 + Vanilla JavaScript
- **Visualization:** SVG (Map Coloring), HTML5 Canvas (Navigation)
- **Algorithms:** CSP Backtracking, BFS, DFS
- **No external dependencies required**
