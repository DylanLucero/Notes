
# Definitions
### Relation
> Let A and B be sets where x ∈ A and y ∈ B. A relation, R is a subset of A x B.
### Enumeration 
> In other words, we take the first element of set A and create new ordered pair with the elements of set B.

ex:
> A = {1,2,3} 
> B = {1,2,3} 
> A x B = {(1,1),(1,2),(1,3),(2,1),(2,2),(2,3),(3,1),(3,2),(3,3)}

#### Notation
x is related to y: x R y or (x,y) ∈ R
x is not related to y: (x,y) ∉ R

# Example
Let A = {1, 2, 3} and let B = {1, 2, 3}

>a) Enumerate A × B
>
>b) Let R be defined on A × B so that (x, y) ∈ R <-> x-y is odd. Determine what ordered pairs of A × B ∈ R.
>
 >c) Draw two mapping diagrams of R. One where A maps to B, and one where A maps to itself.
 
##### Solution

>Using the [[Section 5.1 - Relations and Mapping Diagrams#Definition|definition]] of enumeration, we can enumerate the sets as follows.
>
>  a) A x B = {(1,1),(1,2),(1,3),(2,1),(2,2),(2,3),(3,1),(3,2),(3,3)}
>  
>  R is defined to be an ordered pair (x,y) that is an element of the set R where (x - y) are odd.
>
>  b) R = {(1,2),(2,1),(2,3),(3,2)}
>  
>  Now we need to draw the mapping diagrams for the sets.
>
>c) ![[5.1 - Relations - Enumeration Diagram.drawio.png]]

# Less than or equal to relation

>Let A = {1,2} and let B = {0, 1, 2, 3}. Let x R y if x ≤ y. Find all (x,y) ∈ R  and list R as a set.

>Solution: We will enumerate all of the pairs (x,y) and see which ones satisfy x ≤ y

x | y | x <= y| x R y
:--:|:--:|:--:|:--:
1 | 0 | 1 <= 0 False | No
1 | 1 | 1 <= 1 True | Yes
1 | 2 | 1 <= 2 True | Yes
1 | 3 | 1 <= 3 True | Yes
2 | 0 | 2 <= 0 False | No
2 | 1 | 2 <= 1 False | No
2 | 2 | 2 <= 2 True | Yes
2 | 3 | 2 <= 3 True | Yes

>R = {(1,1),(1,2),(1,3),(2,2),(2,3)}

# Circle Relation

>Define the relation C on R × R  so that (x, y) ∈ C if $x^2+y^2=1.$
>Determine whether the following points belong to R. 

## Solution:
>Recall that our function is: $x^2+y^2=1.$

| Is  |  $$x^2+y^2=1.$$ |   |
|:---:|:---:|:---:|
|1 R 0|Check: $1^2$ + $0^2$ = 1 + 0 = 1|Yes|
|0 R 1|Check: $0^2$ + $1^2$ = 0 + 1 = 1|Yes|
|−1 R 1|Check: $1^2$ + $-1^2$ = 1 + 1 = 2|No|
|$\frac{1}{2}$ R $\frac{\sqrt3}{2}$|Check: $(\frac{1}{2})^2$ + $(\frac {\sqrt 3}{2})^2$ = $\frac {1}{4}$ + $\frac {3}{4}$ = 1 | Yes

>b) What does the graph of C look like in the x – y plane? 
> 
>Answer: The graph is a circle centered at the origin with radius 1.
>
>c) Why is C a relation, but not a function?  
>
>Answer: An input can have more than one output. For example,
>$(\frac{1}{2}$,$-\frac{\sqrt {3}}{2})$ and $(\frac {1}{2}$,$\frac{\sqrt 3}{2})$ are both in R.