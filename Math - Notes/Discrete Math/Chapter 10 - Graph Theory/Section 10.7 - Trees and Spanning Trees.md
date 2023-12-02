# Definitions
A graph G is a **_tree_** if it is circuit free and connected.

A tree is a **_minimally connected graph_**.  The removal of an edge from any tree would make the graph disconnected.

## Theorem 
A graph G that is a tree on n vertices has $n–1$ edges.

## Note
The converse of the theorem is _not_ true.  Having $n-1$ edges does not guarantee a tree.

# Trees

Determine if the following graphs are trees and justify your answer.  
![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638167116799-0.png)  
Solution:

  
a) The first graph is not a tree since it is not connected.

b) The second graph is not a tree since it has a circuit. Also it has 4 vertices and 4 edges. A tree would have 3 edges.

c) The third graph is a tree. It is connected with 6 vertices and 5 edges.
# Spanning Trees


## Definition 
A **_spanning tree_** H is a subgraph of a graph G such that H is a tree, and its vertices and edge sets are subsets of G’s vertices and edge sets.

The graph G below represents a computer network. The 16 vertices represent the computers, and the edges represent the connections between the computers.  
Find a subgraph H that is a spanning tree of G. What is good and bad about changing the computer network to a spanning tree?

![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid40_2.png)

Solution: There are 16 vertices so our tree will have 15 edges. Keep removing edges until there are 15 while ensuring you are not disconnecting the graph.  
I started by removing all the edges between the two identical figures except 1 to keep the pieces connected. Now there are 25 edges. This step is shown below.

![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid41_2.png)

There are 8 vertices in each half, so I want 7 edges to remain in each half. There are currently 12 edges in each half, so I’ll remove 5 on both sides while making sure they do not disconnect. I did the two sides differently to show different possibilities. Note there are 15 edges, the graph is connected, and it is easy to observe there are no cycles (circuits).

![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid42_2.png)

With the spanning tree, the computer network is still connected, but we do not need to use as many materials to connect them which may save money. However, if any single connection fails (an edge is removed) the network will no longer be connected. We call an edge a _**cut point**_ when it has this property. Every edge in a tree is a cut point.  Cut points are problematic in any network.  If you consider the energy grid, you wouldn't want one failure (a squirrel chews through a line in Nebraska) to take down the whole system.  We prefer redundancy.  We prefer redundancy.  Redundancy.