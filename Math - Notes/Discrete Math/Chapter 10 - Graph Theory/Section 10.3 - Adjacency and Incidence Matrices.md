# Definition & Example
Let $G$ be graph on $n$ vertices.  An **_adjacency matrix_** is an $n$ x $n$ matrix where the $a_{ij}$ entry is the number of edges between vertex $v_i$ and $v_j$.  For a digraph, we only count the edges from $v_i$ to $v_j$.  For an undirected graph, we count an edge between $v_i$ and $v_j$ for both entries $a_{ij}$ and $a_{ji}$

a) Construct the adjacency matrix for the digraph below.

![[10.3-Digraph.png]]

## Solution  
Make sure the vertices are labeled.  There are 4 vertices so the adjacency matrix will be a $4$ x $4$ matrix of the form below.

![[10.3 - MatrixForm.png]]

Start with the row for $v_1$ and enter the number of edges going to $v_j$ from $v_1$.  The vertex $v_1$ has one edge directed to $v_3$.  So the first row is 0 0 1 0 as shown below.

![[10.3 - MatrixTopRow.png]]

The vertex $v_2$ has one edge directed to $v_4$.  So the second row is 0 0 0 1.

The vertex $v_3$ has an edge directed to $v_1$ and $v_2$.  So the third row is 1 1 0 0.

The vertex $v_4$ has an edge directed to $v_3$.  So the fourth row is 0 0 1 0.

So the adjacency matrix is

![[10.3 - MatrixActual.png]]

b) Construct the adjacency matrix for the simple graph below.

![[10.3 - SimpleGraph.png]]

Solution:  First label the vertices. The adjacency matrix will be an $8$ x $8$ matrix.

Proceed row by row as before, but since the edges aren’t directed, any two vertices with an edge will count in the matrix.

- $v_1$ is adjacent to $v_2, v_3$, and $v_5$
- $v_2$ is adjacent to $v_1, v_6$, and $v_4$
- $v_3$ is adjacent to $v_1, v_4$, and $v_7$
- $v_4$ is adjacent to $v_2, v_3$, and $v_8$
- $v_5$ is adjacent to $v_1, v_6$, and $v_7$
- $v_6$ is adjacent to $v_2, v_5$, and $v_8$
- $v_7$ is adjacent to $v_3, v_5$, and $v_8$
- $v_8$ is adjacent to $v_4, v_6$ and $v_7$

![[10.3 - SimpleMatrix.png]]

Observe that if you add the entries in any row, the result is the degree of the vertex.  In addition, the adjacency matrix for a simple graph has 0’s on the diagonal and is symmetric.  A symmetric matrix means a_ij = a_ji.  The diagram below shows how the symmetry presents as a reflection across the diagonal for a_37 and a_73.  This shows that the number of edges between v_3 and v_7 is equal regardless of order.

![[10.3 - FinalMatrix.png]]

# Walks
Definition:  Let u and v be two vertices in a graph G.  A **_walk from u to v_** is an alternating sequence of adjacent vertices and edges that starts with u and ends with v.  The **_length of a walk_** is the number of edges traversed.  To represent a walk we list the vertices and edges with no spaces.

Consider the graph G below and specifically the vertices v1 and v3.  A walk from v1 to v3 would list all the consecutive vertices and edges to get from v1 to v3.

![[10.3 - Walks.png]]

A walk of length 2 from v1 to v3 is v1e2v4e6v3

A walk of length 3 from v1 to v3 is v1e1v5e4v4e6v3

A walk of length 4 from v1 to v3 is v1e2v4e6v3e6v4e6v3 (this walk doubles back on edge e6)

**Adjacency Matrices and Walks**

Theorem:  Let G be a graph with vertices v1, v2, …, vn and let A be the n x n adjacency matrix of G.  Then the aij entry of Am gives the number of walks between vi and vj of length m
## Example
Use technology to find A2, A3, A4, and A5.  **[Matrix Calculator LINK](https://keisan.casio.com/exec/system/15782922275976)**  Then answer the questions.

  ![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid7_4.png)                          ![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid8_4.png)

a) How many walks of length 2 are there between v5 and itself? List them.

b) How many walks of length 4 are there between v1 and v3?

c) Observe that the 2nd row (and 2nd column) of A1 through A5 are all [0 1 0 0 0]. Interpret what this means and explain this based on the structure of the graph.

Solution:  This is the image of A in the online matrix calculator.

![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid9_4.png)

These are the powers of A computed by the matrix calculator.

   A2                                                                                                 A3

  ![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid10_4.png)                             
  ![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid11_4.png)

   A4                                                                                A5

  ![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid12_4.png)                               
  ![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid13_3.png)

Solutions: 

a) A2 tells us the number of walks of length 2. The entry a55 = 5 tells us the number of walks of length 2 between v5 and itself. 

To find the 5 walks, first observe that any edge incident on v5 can be taken one vertex away and back to make a walk of length 2 back to v5.  These include the following:

Edge e1:  v5e1v1e1v5

Edge e3:  v5e3v4e3v5

Edge e4:  v5e4v4e4v5

Next observe that there are 2 edges connecting v5 and v4.  Alternating which one is taken away from v5 and back to v5 give us the last two walks.

Edge e3 first:  v5e3v4e4v5

Edge e4 first:  v5e4v4e3v5

Answer:  There are 5 walks of length to from v5 to itself.  They are

v5e1v1e1v5, v5e3v4e3v5, v5e4v4e4v5, v5e3v4e4v5, v5e4v4e3v5

b) Look at entry a13 or a31 in A4. There are 7 walks of length 4 between v1 and v3.

c) v2 has a loop to itself but is otherwise disconnected from the other vertices in the graph. Therefore, v2 can only have walks of any length to itself and there is only one way for these walks to occur.  The walks must loop around repeatedly.