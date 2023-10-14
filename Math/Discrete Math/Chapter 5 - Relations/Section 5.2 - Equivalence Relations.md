# Definitions

>A [[Section 5.1 - Relations and Mapping Diagrams#Definition|relation]] R is _**reflexive**_ if ∀x ∈ A, x R x.
^e4da0b

>A [[Section 5.1 - Relations and Mapping Diagrams#Definition|relation]] R is _**symmetric**_ if ∀x,y ∈ A, if x R y then y R x. 
^23e1e2

>A [[Section 5.1 - Relations and Mapping Diagrams#Definition|relation]] R is _**transitive**_ if ∀x, y, z ∈ A, if x R y
>and y R z, then x R z.
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
>
>Let A = {1, 2, 3}. Let R be defined on A×A so that (x,y) ∈  R ↔ x − y is even. Use definitions to determine whether R is [[Section 5.2 - Equivalence Relations#^e4da0b|reflexive]], [[Section 5.2 - Equivalence Relations#^23e1e2|symmetric]], or [[Section 5.2 - Equivalence Relations#^acf3bd|transitive]].
### Solution



# Example
>Definition: Let A be a set and R a binary relation on A. An equivalence relation is a relation that has the following properties: reflexive, symmetric, and transitive.
>
>Determine whether the relation is an equivalence relation.  
>Let A=Z . Let R be defined on A×A  so that(x,y)∈R↔3∣(x− y). 
>
>Note:  We will use the equivalence 3∣(x−y)  iff 3k=x−y  for some k in Z 
>
>Check Reflexive: A relation R is reflexive if ∀x∈A, x R x.   
>Proof: Let x∈A . So x−x=0 .   For k=0,x−x=3k=3×0 . So xRx  and R is reflexive.
>
>Check Symmetric: A relation R is symmetric if ∀x,y∈A  ,ifxRy then yRx 
>
>Proof: Let x,y∈A . Let xRy . So x−y=3k  for some k∈Z . Now y−x  = −(x−y)=−3k . Let m=−k  for some integer m, then y−x=3m . So yRx  and R is symmetric.
>
>Check Transitive: A relation R is transitive if ∀ x, y, z∈A ,ifxRy and yRz, then xRz.   
>
>Proof: Let x,y,z∈A  and let xRy  and yRz . Since xRy , x−y=3k  for some k∈Z . And since yRz , y−z=3m  for some m∈Z . Observe that  x−y+y−z=x−z . This can be rewritten as x−z=3k+3m=3(k+m) . Let n=k+m  for some n∈Z  then x−z=3n . So xRz . Therefore R is transitive.
>
>Sin R is reflexive, transitive, and symmetric, R is an equivalence relation.