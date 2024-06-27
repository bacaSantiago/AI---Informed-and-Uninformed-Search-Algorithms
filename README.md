# AI - Informed and Uninformed Search Algorithms

---

## Overview:
This Python program explores both informed and uninformed search algorithms to solve various classic AI problems, using breadth-first search (BFS), depth-first search (DFS), and an informed search algorithm (A*). The program covers four different problems: the Sliding Puzzle, the Magic Triangle, the Three Jars problem, and the Missionaries and Cannibals problem. Each problem is approached using different search algorithms, providing insights into their effectiveness and efficiency. These algorithms are fundamental in artificial intelligence and computational problem-solving.

---

### Problem 1: Missionaries and Cannibals Problem
The Missionaries and Cannibals problem involves three missionaries and three cannibals who must cross a river using a boat that can carry one or two people. The goal is to find a way for all six people to cross the river without violating the constraint that the number of cannibals cannot outnumber the number of missionaries on either side of the river.

**State Space Representation:**
The state space is represented by tuples indicating the number of missionaries (M), cannibals (C), and the boat (B) on each side of the river (L for the left bank, R for the right bank).

**Search Algorithm:**
Breadth-first search (BFS) is used to explore, manually, the state space systematically, ensuring the optimal solution is found. The BFS algorithm is implemented to find the solution path from the initial state to the goal state.

---

### Problem 2: Magic Triangle
The Magic Triangle problem requires arranging the numbers 1 to 6 in a triangular pattern such that the sum of each side of the triangle is equal to 10. This problem is approached using both breadth-first search (BFS) and depth-first search (DFS) algorithms.

**Search Algorithms:**
Both BFS and DFS algorithms are implemented to explore the solution space and find valid configurations of numbers that satisfy the conditions of the Magic Triangle problem. BFS explores the search space layer by layer, while DFS explores deeply along a path until reaching a solution.

**Analysis:**
BFS tends to find optimal solutions efficiently in small search spaces, making it suitable for the Magic Triangle problem.

---

### Problem 3: Three Jars Problem
The Three Jars problem involves distributing water between three jars of different capacities to achieve a specific configuration. In this implementation, an informed search algorithm (A*) and an uninformed search algorithm (BFS) are used to find the solution.

**Informed Search (A*):**
A* search algorithm is employed, utilizing a heuristic function based on the absolute difference between the amounts of water in two jars. The objective is to minimize the difference between the amounts of water in the two largest jars, leading to an optimal solution.

**Uninformed Search (BFS):**
Breadth-first search (BFS) algorithm is applied to explore the state space systematically until a solution is found. BFS ensures that the shortest path to the goal state is discovered.

---

### Problem 4: Sliding Puzzle
The sliding puzzle problem is a classic problem in the field of artificial intelligence and computational problem-solving. It involves a grid of numbered tiles where one tile is missing, and the goal is to rearrange the tiles by sliding them into the empty space until they are in a specified order.

#### 3x3 Sliding Puzzle

**A* Algorithm with Manhattan Distance Heuristic**

This implementation uses the A* algorithm with the Manhattan distance heuristic to solve the 8-number (3x3) sliding puzzle. The Manhattan distance heuristic calculates the sum of the distances between the position of each number and its corresponding target position. The program is capable of solving the puzzle efficiently and provides a solution path from the initial state to the goal state.

**A* Algorithm with Misplaced Tiles Heuristic**

Another implementation of the A* algorithm is provided, this time using the misplaced tiles heuristic. The misplaced tiles heuristic counts the number of elements that are in the wrong position compared to the goal state. This implementation offers an alternative heuristic function for comparison.

**Breadth-First Search (BFS)**

Additionally, an implementation using an uninformed search algorithm, Breadth-First Search (BFS), is included. BFS explores all possible states at each level of the search tree before moving to the next level. While BFS guarantees finding the shortest solution path, it may not be as efficient as informed search algorithms for large search spaces.

#### 4x4 Sliding Puzzle

**A* Algorithm with Manhattan Distance Heuristic**

The program also includes an implementation of the A* algorithm with the Manhattan distance heuristic for solving the 15-number (4x4) sliding puzzle. However, due to the increased complexity of the problem and larger search space, finding a solution may take considerable time, especially for randomly generated initial states.

#### Conclusion

For the 3x3 sliding puzzle, both the A* algorithm with the Manhattan distance heuristic and the misplaced tiles heuristic provide efficient solutions. The choice of heuristic depends on factors such as accuracy and computational efficiency.

In terms of efficiency, informed search algorithms like A* with a good heuristic tend to outperform uninformed search algorithms like BFS, especially for larger search spaces.

For the 4x4 sliding puzzle, the A* algorithm with the Manhattan distance heuristic could potentially find a solution, but execution time may vary depending on the complexity of the initial state. Further optimization techniques specific to the 15-number or greater puzzles may include using more advanced heuristics. For example, we could apply techniques to reduce the problem to a lower dimension by solving the first row and column first, as well as rotation methods to optimize the search for solutions. These techniques could reduce the search space and improve the efficiency of the algorithm, allowing solutions to be found in a more reasonable time even on teams with limited resources.

---

### Dependencies:
- Python 3.x
- matplotlib (for visualization)

**Resources:**
- magic_triangle.png (background image for Magic Triangle visualization)
- bfs_tree.png (graphic solution for problem 1)

**Note:** Ensure that the background image (magic_triangle.png) is accessible in the program directory for proper visualization.

---

This program showcases the versatility of search algorithms in solving various problems, from puzzles to logistical challenges, demonstrating their practical applications in artificial intelligence and computational problem-solving domains.