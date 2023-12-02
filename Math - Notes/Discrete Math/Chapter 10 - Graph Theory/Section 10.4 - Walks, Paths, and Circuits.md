Definition:  Let u and v be two vertices in a graph G.  A **_walk from u to v_** is an alternating sequence of adjacent vertices and edges that starts with u and ends with v. 

Definition:  Let u and v be two vertices in a graph G.  A **_path from u to v_** is a walk that does not contain a repeated edge.

Definition:  Let u and v be two vertices in a graph G.  A **_simple_** **_path from u to v_** is a path that does not contain a repeated vertex.

Definition:  Let u be any vertex in a graph G.  A **_closed_** **_walk_** starts and ends at the same vertex.  So it is a walk from u to u.

Definition:  A **_circuit_** is a closed walk that does not contain a repeated edge.

Definition:  A **_simple circuit_** is a circuit that does not repeat a vertex except the first and last.

Here is a handy chart that compares and contrast the requirements.  Note how the questions are phrased.  Just because an edge or vertex **_may_** repeat doesn’t mean it is required.  Just because the start and end vertex **_do not need_** to be the same, doesn’t mean they aren’t.

|   |   |   |   |
|---|---|---|---|
||May an edge repeat?|May a vertex repeat?|Must the start and end vertex be the same?|
|Walk|Yes|Yes|No|
|Path|No|Yes|No|
|Simple Path|No|No|No|
|Closed Walk|Yes|Yes|Yes|
|Circuit|No|Yes|Yes|
|Simple Circuit|No|Only 1st and last|Yes|