There are many types of graphs that have distinguishing properties.  We define some of them below.

# Definitions

A **_directed graph_** or **_digraph_** is a graph where the edges are directed from one vertex to another.  This is denoted by drawing an arrow on the edge in the direction as opposed to just a line for the edge.  The edge is written as an ordered pair instead of a set, ($v_i, v_j$) where the edge is directed from $v_i$ to $v_j$.

A **_simple graph_** is a graph without any loops or parallel edges (only one possible edge between any two vertices)

A **_bipartite graph_** is a graph where the vertices can be partitioned into two sets so that there are no edges between vertices in the same partition.

A **_subgraph_** $H$ or a graph $G$ is a graph where the vertex and edge sets of $H$ are subsets of the vertex and edge sets of $G$

A **_connected graph_** is a graph where for any vertices $v_i$ and $v_j$, there is a sequence of edges that connect $v_i$ and $v_j$.

A **_planar graph_** is a graph that can be drawn in $2$ dimensions so that none of its edges intersect.

A **_complete graph_** is a graph where every pair of vertices in the graph is adjacent.

# Draw Each Type of Graph Example

Draw an example of each type of graph. (Answers can vary for all of the graphs)

a) A digraph

Solution:  

$V(G) =$ {$v_1, v_2, v_3, v_4$}

$E(G) =$ {$e_1, e_2, e_3, e_4, e_5$}

|Edge|Endpoints|
|:--:|:---:|
|$e_1$|($v_3, v_2$)|
|$e_2$|($v_2, v_4$)|
|$e_3$|($v_4, v_3$)|
|$e_4$|($v_3, v_1$)|
|$e_5$|($v_1, v_3$)|

![[10.2-Digraph-ex.png]]

b) A simple graph – no loops and no parallel edges 

![[10.2-Simple-ex.png]]

c) A bipartite graph – A vertex partition into two sets is {$v_1, v_2, v_3$} and {$v_4, v_5$}

![[10.2-Bipartite-ex.png]]

d) A subgraph – $H$ is a subgraph of $G$

![[10.2-SubGraph-ex.png]]

e) $G$ is a connected graph and $H$ is not a connected graph since there is not a path between $v_2$ and $v_3$ to $v_1, v_4, v_5$, and $v_6$.

![[10.2-Connected-ex.png]]

f) A graph drawn in two ways. The graph on the right shows the graph is planar.

![[10.2-Planar-ex.png]]

g) The graphs below are complete graphs on $2, 3$, and $4$ vertices denoted by $K_n$ where $n$ is the number of vertices.

![[10.2-Complete-ex.png]]