# Graphs

Graphs, in Computer Science, refer to a network of objects (nodes) connected by lines (edges).

+ **Nodes** (or vertices) refer to the individual entities in the network. A node can represent a person, a place, a computer or a webpage.
+ **Edges** (or links) refer to the lines connecting the nodes. Each edge defines a relationship between two nodes.

So, Nodes -> Entities and Edges -> Relationship between those entities.

## Types of Graphs

Depending on how the connections work, graphs fall into a few key categories[2]:

- Edge Direction:
    - **Undirected Graph**: Connections go both ways naturally.
    - **Directed Graph**: Connections have a specific direction (shown with arrows).

- Edge Weight:
    - **Unweighted Graph**: Edges simply show that a connection exists, with no numbers attached.
    - **Weighted Graph**: Each edge has a number (a **weight**) attached to it.

## The Adjacency Matrix

The adjacency matrix is a method that a computer can use to store graphs in memory.

> [!info] Adjacency Matrix Guide
> Each node in the graph is given a row and a column. Intersection of the row of one node and the column of another node results in a single "cell" which indicates the connection between those two nodes. The node whose row was taken is the starting node and the node whose column was taken is the ending node. Given this information, assume 4 nodes A, B, C and D:
> 1. If $(A, B) = 0 \land (B, A) = 0$ -> No connection between the nodes.
> 2. If $(A, C) = 0 \land (C, A) = 1$ -> Directed connection from C to A.
> 3. If $(C, D) = 1 \land (C, B) = 2$ -> Cheaper to go from C to D than from C to B.

## Network Algorithms

Once a network is modeled as a graph, algorithms can be run on it. This is used for things like finding the shortest path between two nodes or finding the most optimized path for a specific purpose.

### Dijkstra's Algortihm to Find Shortest Path

1. Set the distance from starting node to 0 and all other nodes to infinite (unreachable).
2. Choose the unvisited node with the smallest distance value ($g$) (will pick the starting node for the first iteration).
3. Check all the neighbours of the current node and update the neighbour node's $g$ value if: $$g(\text{current}) + \text{edge weight} < g(\text{neighbor})$$
4. Mark the current node as visited and repeat from Step 2 until the target node is reached (path found) or all nodes are visited (no path from starting node to target node).