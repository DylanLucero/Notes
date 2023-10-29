# Definition
##### Conditional Statements
Let p and q be statements. The symbolic form "p -> q" is a **conditional statement** that reads "if p then q" or "p implies q". The statement p is called the **HYPOTHESIS or ANTECEDENT**. The statement q is called the **CONCLUSION or CONSEQUENT**.

Some examples of conditional statements are: 
1) If it does not rain then I will go to the beach. 
	Antecedent: It does not rain 
	Consequent: I will go to the beach. 

2) If you are a cat then you are a mammal. 
	Antecedent: You are a cat 
	Consequent: You are a mammal 
	
3) If I live in Scottsdale then I live in Maricopa County. 
	Antecedent: I live in Scottsdale 
	Consequent: I live in Maricopa County.
##### Biconditional Statements
Let p and q be statements. The symbolic form "p <-> q" is a **biconditional statement** that reads "p if and only if q" or "p iff q".

Some examples of biconditional statements are: 
1. I will help you clean your room if and only if you help me mow the lawn.

2. A polygon is a quadrilateral if and only if it has exactly 4 sides.

3. Janice will eat a hamburger if and only if the hamburger is cooked well done.
# Truth table for the Conditional If p then q

A conditional statement of the form p -> q is false only when p is true and q if false. In particular, when a true hypothesis leads to a false conclusion. Otherwise, the conditional statement is true.

|p|q|p -> q|
|:--:|:--:|:--:|
|T|T|T|
|T|F|F|
|F|T|T|
|F|F|T|

There are three rearrangements of the conditional that come up often.
Given the conditional statement p -> q,
1. The **converse** of p -> q is q -> p.
2. The **inverse** of p -> q is ~p -> ~q.
3. The **contrapositive** of p -> q is ~q -> ~p.

Let’s look at the truth tables for these three forms and compare them to p → q 

|p|q|~p| ~q| p → q| q → p| ~p → ~q| ~q → ~p|
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| T |T| F |F| T |T| T |T| 
| T |F |F |T |F |T |T |F|
| F |T |T |F |T |F |F |T|
| F| F |T| T |T| T |T| T| 

Observe that the original conditional statement p → q, is logically equivalent to its contrapositive ~q → ~p. Similarly, the converse q → p and the inverse ~p → ~q, are logically equivalent to one another. Notice that the converse and the inverse are contrapositives to each other so this is consistent. 

However, none of these forms are the negation of p → q, “ ~(p → q)”. Below is the truth table for the negation of p → q. By definition, we take the opposite of the truth values of p → q. 

|p|q|p → q|~(p → q) |
|:--:|:--:|:--:|:--:|
|T|T|T|F| 
|T|F|F|T|
|F|T|T|F|
|F|F|T|F| 

We’d like a form for the negation that doesn’t require performing the conditional first due to the parentheses, but we saw the converse, inverse, and contrapositive do not satisfy the values we need in the truth table. Instead of using a conditional, we can write the negation using a conjunction as shown below. 

The negation of p → q is logically equivalent to p ˄~q. This is verified in the truth table below. 

|p |q| ~q |p → q| ~(p → q)| p ˄ ~q| 
|:--:|:--:|:--:|:--:|:--:|:--:|
|T| T| F| T| F| F| 
|T| F| T| F| T| T|
|F| T| F| T| F| F| 
|F| F| T| T| F| F|

>Fact: The negation of p → q is ~(p → q) ≡ p ˄ ~q

# Truth table for the Biconditional p if and only if q

Truth table for the Biconditional p if and only if q. A biconditional statement of the form p ↔ q is true when p and q have the same truth value and false when p and q have different truth values. 

|p|q|p ↔ q|
|:--:|:--:|:--:|
|T|T|T|
|T|F|F|
|F|T|F| 
|F|F|T|