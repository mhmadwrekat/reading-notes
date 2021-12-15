## Graphs

---
A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

Here is some common terminology used when working with Graphs :

1. Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
2. Edge - An edge is a connection between two nodes.
3. Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge. 
4. Degree - The degree of a vertex is the number of edges connected to that vertex .

---
## Directed vs Undirected

***Undirected Graphs***

An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

For example, in the graph below, Node C is connected to Node A, Node E and Node B. There are no “directions” given to point to specific vertices. The connection is bi-directional.

![example1](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

The undirected graph we are looking at has 6 vertices and 7 undirected edges.

Vertices/Nodes = {a,b,c,d,e,f}

Edges = {(a,c),(a,d),(b,c),(b,f),(c,e),(d,e),(e,f)}


***Directed Graphs (Digraph)***

A Directed Graph also called a Digraph is a graph where every edge is directed.

Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

Compare the visual below with the undirected graph above. Can you see the difference? The Digraph has arrows pointing to specific nodes.

![example2](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DirectedGraph.PNG)

The directed graph above has six vertices and eight directed edges

Vertices = {a,b,c,d,e,f}

Edges = {(a,c),(b,c),(b,f),(c,e),(d,a),(d,e)(e,c)(e,f)}

---
## Complete vs Connected vs Disconnected

There are many different types of graphs. This depends on how connected the graphs are to other node/vertices.

The three different types are completed, connected, and disconnected

1. Complete Graphs
2. Connected
3. Disconnected

---
## Acyclic vs Cyclic

1. Acyclic Graph

An acyclic graph is a directed graph without cycles .

2. Cyclic Graphs

A Cyclic graph is a graph that has cycles .


![Graphs](https://cdn.educba.com/academy/wp-content/uploads/2020/01/Types-of-Graph-in-Data-Structure.png)


---
## Graph Representation

***We represent graphs through :***

- Adjacency Matrix .

An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix .

Each Row and column represents each vertex of the data structure. The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection .

**a sparse** graph is when there are very few connections. a dense graph is when there are many connections


- Adjacency List .

An adjacency list is the most common way to represent graphs .

An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected .

Adjacency lists make it easy to view if one vertices connects to another .

---
## Weighted Graphs

A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights .  

---
## Traversals

You will be required to traverse through a graph. The traversals itself are like those of trees. Below is a breakdown of how you would traverse a graph .

1. Breadth First

Here is what the algorithm breadth first traversal looks like:

- Enqueue the declared start node into the Queue.
- Create a loop that will run while the node still has nodes present.
- Dequeue the first node from the queue
- if the Dequeue‘d node has unvisited child nodes, add the unvisited children to visited set and insert them into the queue.

2. Depth First

The algorithm for a depth first traversal is as follows:

- Push the root node into the stack
- Start a while loop while the stack is not empty
- Peek at the top node in the stack
- If the top node has unvisited children, mark the top node as visited, and then Push any unvisited children back into the stack.
- If the top node does not have any unvisited children, Pop that node off the stack
- repeat until the stack is empty.

--- 
## Real World Uses of Graphs

***Graphs are extremely popular when it comes to it’s uses. Here are just a few examples of graphs in use :***

- GPS and Mapping
- Driving Directions
- Social Networks
- Airline Traffic
- Netflix uses graphs for suggestions of products

> ***There is a lot to graphs, and a lot you can do with them. Let this be document be used as an introduction to graphs. There is a lot more to them then described, so start exploring, and have fun with them!***

---
## Sources and references

- ***[Graphs .](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)***

---
#### **[Back To Home Page](https://mhmadwrekat.github.io/reading-notes)**

---
<b>
<p align="center">
© Mohammad alwrekat
</p>
