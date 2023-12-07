Recall the following definition and theorem from Chapter 10 on Hamiltonian Circuits.

## Definition  
Given a graph G, a [[Section 10.6 - Hamiltonian Circuits#^2cd675|Hamiltonian circuit]] for G is a simple circuit that includes every vertex of G.

## Theorem  
If G has a nontrivial **Hamiltonian circuit**, then G has a subgraph H with the following properties.

1) H contains every vertex of G
2) H is connected
3) H has the same number of vertices as edges
4) Every vertex of H has degree 2

The difficulty with this theorem is that although we can use it to show a graph **_does_** **_not_** have a Hamiltonian circuit, we’d actually have to find the Hamiltonian circuit to show that it **_does_** have a circuit. 

There are certain graph types that are guaranteed Hamiltonian Circuits such as complete graphs on 3 or more vertices.  However, in general, there is no simple check to determine whether or not a graph has a Hamiltonian Circuit.  We would have to enumerate every possible subgraph and check each one. This is time consuming by hand and can even be time consuming for computers if there are a lot of vertices and edges.

Instead, we will focus our energy on finding **_optimal solutions_** to graphs that are known to have Hamiltonian Circuits.  Specifically, we will focus on the traveling salesman problem which uses weighted graphs.

Definition:  A **_weighted graph_** G is a graph where a number corresponds to each edge of the graph.  These numbers are called the weight of the edge and can represent distance, cost, or any quantitative variable of our choosing.

Recall the example from Chapter 10 below.  First, we will build up some strategies for solving this problem with simpler graphs, and then return to this one.

Suppose a salesman needs to give sales pitches in four cities. He looks up the airfares between each city and puts the costs in a graph. In what order should he travel to visit each city once then return home with the lowest cost?  (Source:  [Lippman](http://www.opentextbookstore.com/mathinsociety/2.5/GraphTheory.pdf))

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156436-0.png)

# Brute Force Method
Find all possible Hamiltonian Circuits for the graph below and their corresponding weights.  Then find the minimum weight circuit. (Source:  [Lippman](http://www.opentextbookstore.com/mathinsociety/2.5/GraphTheory.pdf))

![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid0_8.png)

Solution:  Observe that there are 4 vertices and that each vertex in the graph is adjacent to every other vertex of the graph.  Therefore, this is K4, a complete graph on 4 vertices.  There are 3 unique Hamiltonian Circuits for this graph.  (More on this later.)

Starting with vertex A the circuits are:

|   |   |   |
|---|---|---|
|Circuit|Graph|Weight|
|ABCDA|![](https://moer.maricopa.edu/filestore/ufiles/2745/e1.png)|4 + 13 + 8 + 1 = 26|
|ABDCA|![](https://moer.maricopa.edu/filestore/ufiles/2745/e2.png)|4 + 9 + 8 + 2 = 23|
|ACBDA|![](https://moer.maricopa.edu/filestore/ufiles/2745/e3.png)|2 + 13 + 9 + 1 = 25|

**Answer**:  The minimum weight circuit is ABDCA with a weight of 23.

Since this graph was small, exhausting all of the possibilities was easy.  Let’s use combinatorics to see how many circuits there would be larger complete graphs.

In our example, there were 4 vertices for $K_4$.  The number of permutations of 4 objects is 4! = 24.  Since a circuit is essentially a circle, the vertex we start with is irrelevant.  So the following are equivalent.  Verify this by following the paths on the graph below and then returning to the original vertex.

$$ABCD \;\;\;\;        BCDA     \;\;\;\;    CDAB   \;\;\;\;    DABC$$

So this decreases the number of circuits by a factor of 4, or in general for Kn, a factor of n.

Now notice that reversing the order also gives the same circuit.  The correspondence is below.  Verify this by using the graph.

ABCD → DCBA               

BCDA → ADCB       

CDAB → BADC     

DABC→ CBAD

![](https://moer.maricopa.edu/filestore/ufiles/2745/e1_1.png)

So this decreases the number of circuits by a factor of 2 regardless of the n value for Kn.  So our 3 circuits from $K_4$ can be found using t he formula below.

  
$$\frac{4!}{4×2}=\frac{3!}{2}=3$$

In general, $K_n$ has the following number of unique circuits.

$$\frac{n!}{n×2}=\frac{(n−1)!}{2} $$

|   |   |
|---|---|
|**n**|**Unique Hamiltonian Circuits**|
|9|8!/2 = 20,160|
|10|9!/2 = 181,440|
|11|10!/2 = 1,814,400|
|15|14!/2 = 43,589,145,600|
|20|19!/2 = 60,822,550,204,416,000|

As you can see the number of circuits is growing extremely quickly as n increases. If a computer looked at one billion circuits a second, it would still take almost two years to examine all the possible circuits with only 20 cities for the traveling salesman problem. Certainly Brute Force is **_not_** an efficient algorithm.

Unfortunately, no one has yet found an efficient _and_ optimal algorithm to solve the TSP, and it is very unlikely anyone ever will. Since it is not practical to use brute force to solve the problem, we turn instead to _**heuristic algorithms**_; efficient algorithms that give approximate solutions. In other words, heuristic algorithms are fast, but may or may not produce the optimal circuit.

# Nearest Neighbor Algorithm
Next, we will use the Nearest Neighbor Algorithm (NNA).  It does not require finding all possible Hamiltonian Circuits, so it is more efficient.  The steps are listed below.

1) Select a starting point.

2) Move to the nearest unvisited vertex (the edge with smallest weight).

3) Repeat until the circuit is complete.

**Problem 5:  Written Example –** Hamiltonian Circuits – Nearest Neighbor Algorithm

Use the NNA to find a Hamiltonian circuit starting at vertex A.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156457-0.png)

Solution:  We are given the starting point in the problem, vertex A.  Next, draw the edge from A to D since 1 is the smallest weight of a vertex that has not been visited yet.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156457-1.png)

The two remaining vertices are B and C.  The edge weight to vertex C is smaller so draw the edge from D to C.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156457-2.png)

The only remaining vertex that has not been visited is B.  Draw the edge from C to B.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156457-3.png)

Finally, return to vertex A to complete the circuit.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156457-4.png)

Answer:  So the circuit produced by NNA is ADCBA with a weight of 26.

We ended up finding the worst circuit in the graph! What happened? Unfortunately, while it is very easy to implement, the NNA is a **_greedy algorithm_**, meaning it only looks at the immediate decision without considering the consequences in the future. In this case, following the edge AD forced us to use the very expensive edge BC later.

# Sorted Edges Algorithm
We’ll learn one more algorithm for a minimum Hamiltonian circuit called the _**Shortest Edges of Cheapest Link Algorithm.**_ Here are the steps.

  
1) Determine the minimum edge weight in the graph and add the edge to the circuit  
2) Find the next smallest edge weight in the graph and add the edge to the circuit unless either of the following apply:

  
a) If adding the edge would make a circuit that does not include all of the vertices of the graph  
b) If adding the edge would make a vertex have degree 3 (Recall all vertices in an HC have degree 2)

  
If either of the two cases above apply pick the edge with the next smallest edge weight and check the criteria above.

  
3) Repeat until the circuit is complete.

**Problem 7:  Written Example –** Hamiltonian Circuits – Sorted Edges Algorithm

Use the Sorted Edges Algorithm to find a Hamiltonian circuit.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156515-0.png)

Solution:  The minimum edge weight is 1.  Add this edge to the graph.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156515-1.png)

The next smallest edge weight is 2.  Adding this edge does not make a circuit or make a vertex of degree 3 so it meets the criteria.  Add this edge to the graph.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156515-2.png)

The next smallest edge weight is 4.  However, adding this edge would make vertex A have degree 3 which is prohibited.  Do not add this edge and continue the search.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156515-3.png)

The next smallest edge weight is 8.  However, adding this edge would make a circuit with vertices ACD, but not B which is prohibited.  Do not add this edge and continue the search.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156515-4.png)

The next smallest edge weight is 9.  Adding this edge does not make a circuit or make a vertex of degree 3 so it meets the criteria.  Add this edge to the graph.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156515-5.png)

The edge with weight 13 is the one remaining edge that is not prohibited that completes the circuit.  Add the edge.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156515-6.png)

Answer: The Hamiltonian circuit generated by the Sorting Edges Algorithm is ADBCA.

Notice that the algorithm did not produce the optimal circuit in this case; the optimal circuit is ACDBA with weight 23.   While the Sorted Edge algorithm overcomes some of the shortcomings of NNA, it is still only a heuristic algorithm, and does not guarantee the optimal circuit.