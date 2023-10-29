# Definitions
A relation R on a set A is **partial ordering** if it satisfies all three properties below:
1. Reflexivity: $\forall x \in A, a R a$  $\forall x \in A, aRa$
 ^eb23c1
2. Transitivity: $\forall x,y,z \in A$, if $xRy$ and $yRz$ then $xRz$
 ^f7c42e
3. Antisymmertry: $\forall x,y \in A$, if $xRy$ and $yRx$ then $x = y$ ^eb69b5

Notice that the main difference between an equivalence relation and a partial ordering is that equivalence relations have symmetry and partial ordering have antisymmetry. The simplest way to see the idea between antisymmetry is to consider a basic ordering, namely, less than.

For example:
$$3\leq4\;but\;4\nleq3$$
So, reversing the order of a partial order relation causes the relation to no longer hold.

#### Notation
For partial orderings, we use the notation $x\preceq y$ and this reads "x is less than or equal to y" or equivalently "y is greater than or equal to x".

# Differentiating between Equivalence Relations and Partial Order Relations

While both equivalence relations and partial order relations require reflexivity and transitivity, ***an equivalence relation requires symmetry but does not require antisymmetry and Partial order relations require antisymmetry but does not require symmetry***. 

| |Reflexive|Symmetric|Antisymmetric|Transitive|
|:--:|:--:|:--:|:--:|:--:|
|Equivalence Relation|Yes|Yes|No|Yes|
|Partial Order Relation|Yes|No|Yes|Yes|

Let’s look at some examples to help differentiate partial order relations and equivalence relations. 

##### **Example 1:** 
An equivalence relation that is not a partial order relation. 

Let R be defined on Z × Z so that (x, y) ∈ R if and only if 3|x − y. 

Since R is reflexive, symmetric, and transitive, it is an equivalence relation. (See section 5.2 worked example for proof.) 

On the other hand, we can find a counter example that shows R is not antisymmetric. 

(1, 4) ∈ R since 1 − 4 = −3 and 3 | -3. 
(4, 1) ∈ R since 4 − 1 = 3 and 3|3. 

However, 1 ≠ 4. 

This shows that R is not antisymmetric so it can’t be a partial order relation.

##### **Example 2**: 
A partial order relation that is not an equivalence relation 

Let R be defined on the set of all sets so that (A, B) ∈ R if and only if A ⊆ B. 

Since R is reflexive, antisymmetric, and transitive, it is a partial order relation. 

However, we can show that R is not symmetric with a counter example.

Consider the sets A = {1} and B = {1, 2}. 

A ⊆ B so (A, B) ∈ R. 
But $B \not\subset A$, thus $(B,A) \notin R$. 

This means R is not symmetric and not an equivalence relation. 

##### **Example 3**:
A relation that is both a partial order and an equivalence relation. 

The relation commonly referred to as equality, =, is both a partial order relation and an equivalence relation. 

Let’s provide a stricter definition: Define R on R × R such that (x, y) ∈ R if and only if x = y. Can you prove that R is a partial order relation and an equivalence relation? 

Recall that this means showing that R is reflexive, symmetric, antisymmetric, and transitive.