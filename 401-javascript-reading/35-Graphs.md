# Graphs


> A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.


**Terminology**


  *  **Vertex** - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
  * **Edge** - An edge is a connection between two nodes.
  * **Neighbor** - The neighbors of a node are its
   adjacent nodes, i.e., are connected via an edge.
  * **Degree** - The degree of a vertex is the number of edges connected to that vertex.


## Undirected Graphs

>  is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

![undirected](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3d/Undirected_graph.svg/1280px-Undirected_graph.svg.png)


## Directed Graphs (Digraph)

> also called a Digraph is a graph where every edge is directed.


![Directed Graphs (Digraph)](https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Directed_graph.svg/1280px-Directed_graph.svg.png)



## Complete vs Connected vs Disconnected

* **Complete**

> A complete graph is when all nodes are connected to all other nodes.

* **Connected**

> A connected graph is graph that has all of vertices/nodes have at least one edge.


* **Disconnected**

> A disconnected graph is a graph where some vertices may not have edges.


## Acyclic vs Cyclic

**Acyclic Graph**

>An acyclic graph is a directed graph without cycles.

**Cyclic Graphs**

>A Cyclic graph is a graph that has cycles.


**Adjacency Matrix**

An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix


**Adjacency List**

An adjacency list is the most common way to represent graphs.


**Weighted Graphs**

A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights



**This is the code for a breadth first traversal:**


```

ALGORITHM BreadthFirst(vertex)
    DECLARE nodes <-- new List()
    DECLARE breadth <-- new Queue()
    DECLARE visited <-- new Set()

    breadth.Enqueue(vertex)
    visited.Add(vertex)

    while (breadth is not empty)
        DECLARE front <-- breadth.Dequeue()
        nodes.Add(front)

        for each child in front.Children
            if(child is not visited)
                visited.Add(child)
                breadth.Enqueue(child)

    return nodes;

```


[Home](../README.md)

