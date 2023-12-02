# Definitions
A _**graph**_ $G$ with $n$ vertices and $m$ edges consists of a **vertex set** $V(G) = {v_1, v_2, …, v_n}$ and an edge set $E(G) = {e_1, e_2, …, e_m}$. 

Each edge consists of one or more vertices called its _**endpoints**_. 

If two vertices are endpoints of the same edge, we say the vertices are _**adjacent**_. 

An edge is called _**incident**_ on the vertices that are its endpoints. 

An edge that is incident to only one endpoint is called a _**loop**_. 

If there are two different edges that have the identical endpoints, the edges are called _**parallel**_. 

A vertex on which no edges are incident is called an _**isolated vertex**_. 

The _**degree of a vertex**_ $v_i$, denoted $deg(v_i)$ is the number of edges incident on $v_i$. 

The _**total degree of G**_ is the sum of all the degrees of the vertices of $G$.

# Basics of a Graph Example
Use the graph G below to answer the questions.

![[10.1-ex.png]]

a) Find the vertex set of $G$.  
b) Find the edge set of $G$.  
c) Create a table stating each edge and its corresponding endpoints in $G$.  
d) List all the vertices that are adjacent to $v_4$ in $G$.  
e) List the edges that are incident on $v_5$ in $G$.  
f) List any loops in $G$.  
g) List any parallel edges in $G$.  
h) List any isolated vertices in $G$.  
i) Find the degree of each vertex and the total degree of $G$.

## Solutions
a) We use the notation $V(G)$ to represent the vertex set of $G$. List all the vertices in $G$ in set notation.  
Answer: $V(G) = {v_1, v_2, v_3, v_4, v_5}$

b) We use the notation $E(G)$ to represent the edge set of $G$. List all the edges in $G$ in set notation.  
Answer: $E(G) = {e_1, e_2, e_3, e_4, e_5, e_6}$

c) Make a table with $2$ columns and list the edges on the left and the corresponding endpoints as a set on the right.

| Edge | Endpoints  |
| :--: | :--: |
| $e1$ | {$v_1, v_5$} |
| $e2$ | {$v_1, v_4$} |
| $e3$ | {$v_4, v_5$} |
| $e4$ | {$v_4, v_5$} |
| $e5$ | {$v_2$}     |
| $e6$ | {$v_3, v_4$} |

d) Look at the graph and determine what vertices are connected to $v_4$ by an edge.  
Answer: $v_1, v_3, v_5$

e) Look at the graph and determine what edges are incident on $v_5$.  
Answer: $e_1, e_3, e_4$

f) There is one edge that is incident on only one vertex.  
Answer: $e_5$ is a loop

g) There is one pair of distinct edges that are incident on the same vertices.  
Answer: $e_3$ and $e_4$ are parallel

h) $v_2$ seems like a good candidate for an isolated vertex since it is not connected to the rest of the graph. However, the formal definition is that an isolated vertex is a vertex on which _**no edges**_ are incident. Since $e_5$ is incident on $v_2$, so $v_2$ is not isolated. All of the other vertices have edges incident on them as well.  
Answer: There are no isolated vertices.

i) Count how many end segments of edges that are incident on each vertex.  

![[10.1-ex-2.png]]
$$deg(v_1) = 2, deg(v_2) = 2, deg(v_3) = 1, deg(v_4) = 4, deg(v_5) = 3$$

Sum the results to find the total degree of $G$  
total degree of $G = 2 + 2 + 1 + 4 + 3 = 12$

  
Fact: The total degree of a graph is always even. This is because any edge is incident on exactly two vertices, so the total degree is 2 times the number of edges, and even number.

# Drawing a Graph Example

Given the vertex set, edge set, and endpoint table below, graph and label the following graph.

$V(G) =$ {$v_1, v_2, v_3, v_4, v_5$}

$E(G) =$  {$e_1, e_2, e_3, e_4, e_5, e_6$}

|Edge|Endpoints|
|:--:|:--:|
|$e_1$|{$v_1, v_3$}|
|$e_2$|{$v_1, v_2$}|
|$e_3$|{$v_3, v_5$}|
|$e_4$|{$v_4, v_5$}|
|$e_5$|{$v_2, v_4$}|
|$e_6$|{$v_4$}|

## Solution
It is likely that two people drawing this graph will have different looking pictures. It all depends on how you initially place and label your vertices. If the graph has the vertices and edges as described, it will be correct and mathematically equivalent to any other graph that meets the criteria.

First draw and label the vertices. Leave some space between them so the graph is easier to read. A circle or polygon shape usually works well. Also label the graph. We usually use $G$, or $H$ if $G$ is taken. One way to do this is shown below on the left.

Next use the edge endpoint table to draw the edges and label them. The completed graph is shown below on the right.


![[10.1-Drawing-1.png]]![[10.1-Drawing-2.png]]