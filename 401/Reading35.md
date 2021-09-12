# Graph

- A graph is a non-linear data structure, and collection of *nodes* and *edges* that represents relationships.
    - Edge - An edge is a connection between two nodes.
    - Nodes are vertices that correspond to objects.

- **terminology used when working with Graphs:**
    - Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
    - Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
    - Degree - The degree of a vertex is the number of edges connected to that vertex.


### Directed vs Undirected
1. Undirected graphs
    - *Undirected graphs* have edges that do not have a direction.

    ![Undirected graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

2. Directed Graphs (Digraph)
    - A *Directed Graph* also called a *Digraph* is a graph where every edge is directed.

    ![Directed Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DirectedGraph.PNG)

### Complete vs Connected vs Disconnected

1. Complete Graphs
    - A complete graph is when all nodes are connected to all other nodes.
2. Connected
    - A connected graph is graph that has all of vertices/nodes have at least one edge.
3. Disconnected
    - A disconnected graph is a graph where some vertices may not have edges.

### Acyclic vs Cyclic
1. Acyclic Graph
    - An acyclic graph is a directed graph without cycles. 

> Note: A cycle is when a node can be traversed through and potentially end up back at itself.

2. Cyclic Graphs
    - A Cyclic graph is a graph that has cycles.
    - Here the cycle is defined as a path of a positive length that starts and ends at the same vertex.

### Graph Representation
1. Adjacency Matrix

- An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix.
- Each Row and column represents each vertex of the data structure. The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection.

2. Adjacency List
- An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.

### Resources
- [Graph](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)