# Breadth-First Search (BFS) – Pseudocode

This document outlines the pseudocode for the **Breadth-First Search (BFS)** algorithm, commonly used for graph traversal and shortest path discovery in unweighted graphs.

---

## Function Definition

```plaintext
Function BFS(Graph G, Node Start_Node):
    Input: 
        G – A graph represented as an adjacency list or matrix.
        Start_Node – The node from which traversal begins.

    Output: 
        A list of nodes visited in BFS order, and optionally,
        the shortest path from Start_Node to all reachable nodes.

    Step 1: Initialize
        - Create an empty queue Q
        - Create a Set/Array 'Visited' to keep track of visited nodes
        - (Optional) Create a Map 'Predecessor' to track paths

    Step 2: Begin traversal
        - Mark Start_Node as visited
        - Enqueue Start_Node into Q

    Step 3: Main Loop
        While Q is not empty:
            a. Dequeue the front node v from Q
            b. For each neighbor u of v:
                i. If u is not in Visited:
                    - Mark u as visited
                    - Record Predecessor[u] = v (for path reconstruction)
                    - Enqueue u into Q

    Step 4: (Optional) Path Recovery
        - To reconstruct the shortest path from Start_Node to any node,
          follow the Predecessor map backwards from the target node.

    Return the list of visited nodes (and Predecessor map if used)
