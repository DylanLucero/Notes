Recall the following definitions and theorem from chapter 10.

Definition:  A graph G is a **_tree_** if it is circuit free and connected.

Definition:  A tree is a **_minimally connected graph_**.  The removal of an edge from any tree would make the graph disconnected.

Theorem:  A graph G that is a tree on n vertices has n – 1 edges.

We found some spanning trees in Chapter 10.  Our method was to remove edges until we have n – 1 edges while ensuring that any edge removal would not disconnect the graph.  In this section, our goal is to find a spanning tree on a weighted graph that minimizes the weight of the tree.  Consider the following problem that necessitates such a tree.

**Example:** (Source:  [Lippman](http://www.opentextbookstore.com/mathinsociety/2.5/GraphTheory.pdf))  A company requires reliable internet and phone connectivity between their five offices (named A, B, C, D, and E for simplicity) in New York, so they decide to lease dedicated lines from the phone company. The phone company will charge for each link made. The costs, in thousands of dollars per year, are shown in the graph.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156598-0.png)

In this case, we don’t need to find a circuit, or even a specific path; all we need to do is make sure we can make a call from any office to any other. In other words, we need to be sure there is a path from any vertex to any other vertex.

Of course, any random spanning tree isn’t really what we want. We want the minimum cost spanning tree (MCST).

**Definition:**  The **_minimum cost spanning tree_** is the spanning tree with the smallest total edge weight.

Remarkably, **_Kruskal’s algorithm_** is both optimal and efficient; we are guaranteed to always produce the optimal MCST.  The steps are below.

1) Select the cheapest unused edge in the graph.

2) Repeat step 1, adding the cheapest unused edge, unless adding the edge would create a circuit

3) Repeat until a spanning tree is formed

# Kruskal's Algorithm
A company requires reliable internet and phone connectivity between their five offices (named A, B, C, D, and E for simplicity) in New York, so they decide to lease dedicated lines from the phone company. The phone company will charge for each link made. The costs, in thousands of dollars per year, are shown in the graph. (Source: Lippman)

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156613-0.png)  
  
Solution: Observe that the graph has 5 vertices, so we need 4 edges. The cheapest edge is $4 (in 1000’s of dollars per year)

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156613-1.png)  
Next cheapest edge is $5 (in 1000’s of dollars per year)

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156613-2.png)  
  
The next cheapest edge is $6 (in 1000’s of dollars per year) but creates a circuit. Skip it.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156613-3.png)  
  
Next cheapest edge is $7 (in 1000’s of dollars per year)

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156613-4.png)  
  
Next cheapest edge is $8 (in 1000’s of dollars per year)

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156613-5.png)  
  
We have 4 edges and a spanning tree of minimum weight as shown below.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638552156613-6.png)  
Answer: The minimum cost per year is $24,000.