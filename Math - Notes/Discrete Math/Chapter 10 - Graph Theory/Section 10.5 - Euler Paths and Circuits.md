In this section, we will introduce the concept of Euler paths and circuits. We will use algorithms to find them in the next chapter.

**Introduction: The Seven Bridges of Konigsberg (Source: [Levin](http://discrete.openmathbooks.org/dmoi3/ch_graphtheory.html))**

In the time of Euler, in the town of Königsberg in Prussia, there was a river containing two islands. The islands were connected to the banks of the river by seven bridges (as seen below). The bridges were very beautiful, and on their days off, townspeople would spend time walking over the bridges. As time passed, a question arose: was it possible to plan a walk so that you cross each bridge once and only once? Euler was able to answer this question. Are you?

![](https://moer.maricopa.edu/filestore/ufiles/2745/Konis.png)

  
The problem above, known as the Seven Bridges of Königsberg, is the problem that originally inspired graph theory. Consider a “different” problem: Below is a drawing of four dots connected by some lines. Is it possible to trace over each line once and only once (without lifting up your pencil, starting and ending on a dot)?

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638167116745-1.png)

There is an obvious connection between these two problems. Any path in the dot and line drawing corresponds exactly to a path over the bridges of Königsberg.

## Definition 
An _**Euler path**_, in a graph or multigraph, is a walk through the graph which uses every edge exactly once.   ^1f73f5

An _**Euler circuit**_ is an Euler path which starts and stops at the same vertex. Our goal is to find a quick way to check whether a graph (or multigraph) has an Euler path or circuit. ^a34b00


If we start at a vertex and trace along edges to get to other vertices, we create a walk through the graph. More precisely, a walk in a graph is a sequence of vertices such that every vertex in the sequence is adjacent to the vertices before and after it in the sequence. If the walk travels along every edge exactly once, then the walk is called an Euler path (or Euler walk). If, in addition, the starting and ending vertices are the same (so you trace along every edge exactly once and end up where you started), then the walk is called an Euler circuit (or Euler tour). Of course if a graph is not connected, there is no hope of finding such a path or circuit. For the rest of this section, assume all the graphs discussed are connected.

The bridges of Königsberg problem is really a question about the existence of Euler paths. There will be a route that crosses every bridge exactly once if and only if the graph below has an Euler path:  
![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638167116745-1.png)  
This graph is small enough that we could actually check every possible walk that does not reuse edges, and in doing so convince ourselves that there is no Euler path (let alone an Euler circuit). On small graphs which do have an Euler path, it is usually not difficult to find one. Our goal is to find a quick way to check whether a graph has an Euler path or circuit, even if the graph is quite large.

One way to guarantee that a graph does not have an Euler circuit is to include a “spike,” a vertex of degree 1.  
![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638167116745-3.png)  
The vertex a has degree 1, and if you try to make an Euler circuit, you see that you will get stuck at the vertex. It is a dead end. That is, unless you start there. But then there is no way to return, so there is no hope of finding an Euler circuit. There is however an Euler path. It starts at the vertex a,a, then loops around the triangle. You will end at the vertex of degree 3.

You run into a similar problem whenever you have a vertex of any odd degree. If you start at such a vertex, you will not be able to end there (after traversing every edge exactly once). After using one edge to leave the starting vertex, you will be left with an even number of edges emanating from the vertex. Half of these could be used for returning to the vertex, the other half for leaving. So you return, then leave. Return, then leave. The only way to use up all the edges is to use the last one by leaving the vertex. On the other hand, if you have a vertex with odd degree that you do not start a path at, then you will eventually get stuck at that vertex. The path will use pairs of edges incident to the vertex to arrive and leave again. Eventually all but one of these edges will be used up, leaving only an edge to arrive by, and none to leave again.

What all this says is that if a graph has an Euler path and two vertices with odd degree, then the Euler path must start at one of the odd degree vertices and end at the other. In such a situation, every other vertex must have an even degree since we need an equal number of edges to get to those vertices as to leave them. How could we have an Euler circuit? The graph could not have any odd degree vertex as an Euler path would have to start there or end there, but not both. Thus for a graph to have an Euler circuit, all vertices must have even degree.

The converse is also true: if all the vertices of a graph have even degree, then the graph has an Euler circuit, and if there are exactly two vertices with odd degree, the graph has an Euler path. To prove this is a little tricky, but the basic idea is that you will never get stuck because there is an “outbound” edge for every “inbound” edge at every vertex. If you try to make an Euler path and miss some edges, you will always be able to “splice in” a circuit using the edges you previously missed.

Since the bridges of Königsberg graph has all four vertices with odd degree, there is no Euler path through the graph. Thus there is no way for the townspeople to cross every bridge exactly once.

**Theorem**: If a graph has an _**Euler circuit**_, then every vertex of the graph has even degree.

**Contrapositive**: If there exists a vertex in a graph that has an odd degree, the then graph does not have an Euler circuit.

**Theorem: (stronger)** A graph G has an _**Euler circuit**_ if and only if G is connected and every vertex of G has even degree.

**Theorem**: A graph G has an _**Euler path**_ if and only if G is connected and has at most two vertices of G have odd degree.

You can attempt to find such paths and circuits without an algorithm, but we will learn an algorithm for finding Euler paths and circuits in the next chapter.

Seven bridges of Konigsberg result: Since all the vertices have odd degree, there is neither an Euler path nor an Euler circuit.