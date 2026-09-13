# AI Search Visualizer

### Interactive visualization of classical AI search algorithms

Explore how different search strategies navigate a problem space, expand nodes, manage the frontier, and discover a path toward a goal.

The **AI Search Visualizer** provides an interactive way to understand and compare both **uninformed** and **informed search algorithms** through visual, step-by-step execution.

---

## Preview

<p align="center">
  <img src="./assets/cover.png" alt="AI Search Visualizer" width="100%">
</p>

<p align="center">
  <b>See how different AI search strategies explore the same problem space in completely different ways.</b>
</p>

---

## Overview

Search is one of the fundamental concepts in Artificial Intelligence.

Given an initial state and a goal, a search algorithm determines how to explore the available states until it finds a solution.

This project turns that process into an interactive visualization.

Instead of only looking at pseudocode or mathematical definitions, you can watch algorithms:

- Explore nodes
- Maintain their frontier
- Backtrack when necessary
- Use path costs
- Apply heuristic estimates
- Discover the goal
- Construct the final path

The visualizer makes it easier to understand **why different algorithms behave differently**, even when solving the same problem.

---

# Search Algorithms

The visualizer currently includes **10 classical AI search algorithms**, divided into two major categories.

---

## 01 — Uninformed Search

> Search strategies that have no additional knowledge about where the goal is.

### Breadth-First Search — BFS

Explores nodes level by level.

BFS prioritizes the shallowest unexplored nodes before moving deeper into the search space.

**Key idea:**  
> Search wide before going deep.

**Useful when:**
- Every action has the same cost
- The shallowest solution is preferred

---

### Depth-First Search — DFS

Explores one branch as deeply as possible before backtracking.

**Key idea:**  
> Go deep before exploring alternatives.

DFS can reach deep solutions quickly, but it does not guarantee the shortest path.

---

### Uniform Cost Search — UCS

Expands the node with the lowest accumulated path cost.

Unlike BFS, UCS considers the actual cost of reaching each state.

**Key idea:**  
> Always expand the cheapest path discovered so far.

---

### Depth-Limited Search — DLS

A variation of DFS that prevents exploration beyond a specified depth.

**Key idea:**  
> DFS with a maximum depth boundary.

This prevents the algorithm from searching indefinitely down a deep branch.

---

### Iterative Deepening DFS — IDDFS

Repeatedly performs depth-limited searches while increasing the depth limit.

For example:

```text
Depth 0
   ↓
Depth 1
   ↓
Depth 2
   ↓
Depth 3
   ↓
...
