In this section, we will introduce the concept of Hamiltonian circuits.  We will use algorithms to find them in the next chapter.

**The Traveling Salesman Problem**

Hamiltonian Circuits apply to a famous problem called the traveling salesman problem.  Here is an example. (Source:  **[Lippman](http://www.opentextbookstore.com/mathinsociety/2.5/GraphTheory.pdf))**

Suppose a salesman needs to give sales pitches in four cities. He looks up the airfares between each city and puts the costs in a graph. In what order should he travel to visit each city once then return home with the lowest cost?

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638167116780-0.png)

In this problem, we are not interested in traversing every edge like we did with Euler circuits.  Instead we want to visit every vertex.  In addition, we don’t want to repeat a vertex.  Once the salesman visits LA, there is no reason to fly back there. There are many algorithms to find solutions which we will learn in the next chapter.  However, they do not necessarily produce optimal solutions in the context of cost.  For now, we will focus on the basics of the structure.

Definition:  Given a graph G, a **_Hamiltonian circuit_** for G is a simple circuit that includes every vertex of G.

Theorem:  If G has a nontrivial Hamiltonian circuit, then G has a subgraph H with the following properties.

a) H contains every vertex of G

b) H is connected

c) H has the same number of vertices as edges

d) Every vertex of H has degree 2

The graphs G and H below display this idea.  G has many edges including the edges drawn in pink.  H is the subgraph of pink edges and the corresponding vertices.  Observe how H meets the four criteria in the theorem.

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638167116780-1.png)