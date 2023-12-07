I this chapter we are going to study algorithms. In particular, we are going to learn a few algorithms from [[Section 10.1 - Definitions and Terminology|Graph Theory]] for finding graph types and graph optimization. We will discuss methods of counting the number of operations in algorithms, and methods for estimating the long-term behavior of the number of operations in algorithms.

Recall the following definitions and theorems from Chapter 10 on Euler paths and circuits.

# Definitions
## Euler Path
An [[Section 10.5 - Euler Paths and Circuits#^1f73f5|Euler Path]] in a graph or multigraph, is a walk through the graph which uses every edge exactly once.

## Euler Circuit
An [[Section 10.5 - Euler Paths and Circuits#^a34b00|Euler Circuit]] is a Euler Path which starts and stops at the same vertex.

## Theorems
A graph G has an Euler Circuit iff. G is connected  and every vertex of G has an even degree

A graph G has an Euler Path iff. G is connected and exactly 2 vertices of G have an odd degree

# Fleury's Algorithm
1) If you are looking for an Euler Circuit, you may start at any vertex. If you are looking for an Euler Path, you must start with one of the two vertices of odd degree. **Write down the vertex**
2) Pick an edge that is adjacent to your starting vertex that will not disconnect the graph into two subgraphs with edges if you remove it. **Write down the vertex after the starting vertex** and remove the edge from your graph (this is how you know you have "covered" this edge already).
3) The last vertex in your list is your new "starting vertex". Repeat the process in 2 for this vertex.
4) Continue in this manner until all edged have been removed.

Your ordered list of vertices will be an Euler Circuit/Path.

## Examples
Use a theorem to verify whether the graph has an Euler path or an Euler circuit.  Then use Fleury’s algorithm to find whichever exists.  (Source:  [Lippman](http://www.opentextbookstore.com/mathinsociety/2.5/GraphTheory.pdf))

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156413-0.png)

Solution: Observe the graph below with its vertices labeled by degree. There are exactly 2 vertices of odd degree, so an Euler path exists.  
![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid0_9.png)  
Since we have an Euler path, we must begin and end at a vertex of odd degree. I will begin at vertex D. I will use the edge incident to A and remove it from the graph. Our path so far is DA.  
![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid1_7.png)  
Next, I will use the edge from A to B and remove it from the graph. Our path so far is DAB.  
![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid2_7.png)  
We only have one edge choice, from B to D. Remove it from the graph. Our path so far is DABD.

![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid3_7.png)

  
We only have one edge choice, from D to C. Remove it from the graph. Our path so far is DABDC.

![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid4_6.png)  
Note we must go from C to A. Since we have a path, we must end the path at E. Remove it from the graph. Our path so far is DABDCA.  
![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid5_6.png)  
Return back to C from A. Our path is DABDCAC  
![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid6_6.png)  
Finally, travel from C to E, completing the path. DABDCACE  
![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid7_6.png)  
Answer: The Euler path is DABDCAC