# Graph Theory Algorithms and Concepts

This repository contains implementations and explanations of various graph theory algorithms and concepts in Python. Whether you're a student studying graph theory or a developer looking to implement these algorithms in your project, this repository aims to provide clear and concise implementations along with explanations for each algorithm.

## Table of Contents

1. [Introduction](#introduction)
2. [Algorithms Covered](#algorithms-covered)
3. [File Structure](#file-structure)
4. [Usage](#usage)
5. [Contributing](#contributing)
6. [License](#license)

## Introduction

Graph theory is a fundamental area of computer science and mathematics that deals with the study of graphs, which are mathematical structures used to model pairwise relations between objects. Graphs consist of vertices (nodes) and edges that connect these vertices. Graph theory has numerous applications in various fields such as computer networking, biology, social sciences, and more.

In this repository, we cover several important graph theory algorithms and concepts, including shortest path algorithms like Dijkstra's algorithm, Bellman-Ford algorithm, Floyd-Warshall algorithm, minimum spanning tree algorithms like Kruskal's algorithm, Prim's algorithm, and graph traversal algorithms like Breadth-First Search (BFS) and Depth-First Search (DFS).

## Algorithms Covered

- Dijkstra's Algorithm: Finds the shortest path between nodes in a graph with non-negative edge weights.
- Kruskal's Algorithm: Finds a minimum spanning tree for a connected, weighted graph.
- Prim's Algorithm: Finds a minimum spanning tree for a connected, weighted graph.
- Bellman-Ford Algorithm: Finds the shortest path between nodes in a graph with negative edge weights or cycles.
- Floyd-Warshall Algorithm: Finds the shortest paths between all pairs of vertices in a weighted graph.
- Breadth-First Search (BFS): Explores a graph level by level, visiting all nodes at each level before moving to the next.
- Depth-First Search (DFS): Explores a graph by going as deep as possible along each branch before backtracking.

## File Structure

```
graph-theory-algorithms/
│
├── dijkstra.py
├── kruskal.py
├── prim.py
├── bellman_ford.py
├── floyd_warshall.py
├── bfs.py
├── dfs.py
├── utils.py
├── README.md
└── LICENSE
```

## Usage

Each algorithm implementation is provided as a standalone Python file. You can simply run these files using a Python interpreter to see the algorithm in action or integrate them into your own projects as needed.

For example, to use Dijkstra's algorithm to find the shortest path between nodes in a graph, you can import the `dijkstra` function from `dijkstra.py` and provide the graph and source node as input:

```python
from dijkstra import dijkstra

# Example graph represented as an adjacency list
graph = {
    'A': {'B': 2, 'C': 5},
    'B': {'C': 1, 'D': 2},
    'C': {'D': 4},
    'D': {'C': 3}
}

# Find shortest path from node 'A' to other nodes
shortest_paths = dijkstra(graph, 'A')
print(shortest_paths)
```

## Contributing

Contributions are welcome! If you find any issues with the implementations or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
