# Definitions

>A [[Section 5.1 - Relations and Mapping Diagrams#Definition|relation]] R is _**reflexive**_ if ∀x ∈ A, x R x.
>![[Reflexive.png]]
^e4da0b

>A [[Section 5.1 - Relations and Mapping Diagrams#Definition|relation]] R is _**symmetric**_ if ∀x,y ∈ A, if x R y then y R x. 
>![[symmetric.png]]
^23e1e2

>A [[Section 5.1 - Relations and Mapping Diagrams#Definition|relation]] R is _**transitive**_ if ∀x, y, z ∈ A, if x R y and y R z, then x R z.
>![[Transitive.png]]
^acf3bd

>>>Note: Since these three properties have universal quantifiers, their negations are existential quantifiers.

>A [[Section 5.1 - Relations and Mapping Diagrams#Definition|relation]] R is _**not reflexive**_ if ∃x ∈ A  such that x is not related to x.  
^f33051

>A [[Section 5.1 - Relations and Mapping Diagrams#Definition|relation]] R is _**not symmetric**_ if ∃x,y ∈ A, such that x is related to y, but y is not related to x.  
^29348f

>A [[Section 5.1 - Relations and Mapping Diagrams#Definition|relation]] R is _**not transitive**_ if ∃x, y, z ∈ A, such that x is related to y, y is related to z, but x is not related to z.
^0b2d5f

# Example
>a) Let A = {1, 2, 3) Let R be defined on A × A so that x R y if x ≤ y. Use a mapping diagram to determine whether R is [[Section 5.2 - Equivalence Relations#^e4da0b|reflexive]], [[Section 5.2 - Equivalence Relations#^23e1e2|symmetric]], or [[Section 5.2 - Equivalence Relations#^acf3bd|transitive]].

>b) Let A = {1, 2, 3}. Let R be defined on A×A so that (x,y) ∈  R ↔ x − y is even. Use definitions to determine whether R is [[Section 5.2 - Equivalence Relations#^e4da0b|reflexive]], [[Section 5.2 - Equivalence Relations#^23e1e2|symmetric]], or [[Section 5.2 - Equivalence Relations#^acf3bd|transitive]].
### Solution

In order for us to determine if our set R is reflexive, symmetric or transitive, we need to draw out a mapping diagram.

Since we are doing A x A, we  can draw the diagram as such:
a) Let A = {1, 2, 3) Let R be defined on A × A so that x R y if x ≤ y.
![[5.2-example-a.png]]
Taking a look at the diagram, we can see that A x A with the restraint of x <= y is both [[Section 5.2 - Equivalence Relations#^e4da0b|reflexive]] and [[Section 5.2 - Equivalence Relations#^acf3bd|transitive]].

b) Let A = {1, 2, 3}. Let R be defined on A×A so that (x,y) ∈  R ↔ x − y is even. 

Using definitions, we need to check if the set R is reflexive, symmetric or transitive

Check reflexive: A relation R is reflexive if for all x in A, x relates to x.
>Proof: Let x be any element of A. So x - x = 0, which is an even number. So x R x and R is reflexive.

Check symmetric: A relation R is symmetric if for all x,y in A, if x R y then y R x.
>Proof: Let x,y be any elements of A. Let x R y. So x - y = 2k for some integer k. Now y - x = -(x - y) = -2k. Let m = -k for some integer m, then y - x = 2m. so y R x and R is symmetric.

Check transitiveL A relation R is transitive if for all x,y,z in A, if x R y and y R z, then x R z.
>Proof: Let x,y,z be any elements of A and let x R y and y R z. Since x R y, x - y = 2k for some integer k. And since y R z, y - z = 2m for some integer m. Observe that x - y + y - z = x - z. This can be rewritten as x - z = 2k + 2m = 2 (k + m). Let n = k + m for some integer n. Then x - z = 2n. So x - z is even and x R z. Therefore R is transitive.
# Example

Definition: Let A be a set and R a binary relation on A. An equivalence relation is a relation that has the following properties: reflexive, symmetric, and transitive.

Determine whether the relation is an equivalence relation.  
Let A=Z . Let R be defined on A×A  so that(x,y)∈R↔3∣(x− y). 

>>Note:  We will use the equivalence 3∣(x−y)  iff 3k=x−y  for some k in Z 

Check Reflexive: A relation R is reflexive if ∀x∈A, x R x.   
>Proof: Let x∈A . So x−x=0 .   For k=0,x−x=3k=3×0 . So xRx  and R is reflexive.

Check Symmetric: A relation R is symmetric if ∀x,y∈A  ,if xRy then yRx 
>Proof: Let x,y∈A . Let xRy . So x−y=3k  for some k∈Z . Now y−x  = −(x−y)=−3k . Let m=−k  for some integer m, then y−x=3m . So yRx  and R is symmetric.

Check Transitive: A relation R is transitive if ∀ x, y, z∈A ,if xRy and yRz, then xRz.   
>Proof: Let x,y,z∈A  and let xRy  and yRz . Since xRy , x−y=3k  for some k∈Z . And since yRz , y−z=3m  for some m∈Z . Observe that  x−y+y−z=x−z . This can be rewritten as x−z=3k+3m=3(k+m) . Let n=k+m  for some n∈Z  then x−z=3n . So xRz . Therefore R is transitive.

Sin R is reflexive, transitive, and symmetric, R is an equivalence relation.