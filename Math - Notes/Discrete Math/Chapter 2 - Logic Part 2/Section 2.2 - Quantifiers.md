# Definitions
**Universal Quantifier:**
The **universal quantifier**, $\forall$, states that a predicate is true for all members of its domain.

**Universal Statement:**
Given a predicate $P(x)$ and a domain $D$, a **universal statement** of the form "$(\forall x)P(x)$" or "$\forall x \in D,\; P(x)$" states that a predicate is true for all elements x in the domain D.

**Existential Quantifier:**
The **existential quantifier**, $\exists$, states that there exists an element in the domain $D$ for which the predicate is true.

**Existential Statement:**
Given a predicate $P(x)$ and a domain $D$, an **existential statement** of the form "$(\exists x)P(x)$" or "$\exists x \in D,\; P(x)$" states that there exists an element x in the domain D for which $P(x)$ is true.
# Proving or Disproving an Existential Statement or a Universal Statement
1) You can prove an existential statement by showing that one element in the domain satisfies the predicate. 

	Statement: There exists an even number that is divisible by 7. 

	Domain: The set of even numbers n. 
	Predicate: $n$ is divisible by $7$.

	Since $14$ is even and $14$ is divisible by $7$, there exists an even number that is divisible by $7$.

2) For small domains, you can disprove an existential statement by showing that all of the elements in the domain do not satisfy the predicate. This is called the **method of exhaustion**. 

	Statement: Let $S = {1, 3, 5}$ There exists an element in $S$ that is even.
	
	A number is even if it can be written as a product of $2$ and another integer. For $S$, $$1=2*1─1\;\;\;\;\;\; 3=2*2─1\;\;\;\;\;\;\;5=2*3─1$$ Since each number in S is one less than a multiple of 2, no element in S is even. 
	
	Therefore, it is false that there exists an element in S that is even. 

3) You can disprove a universal statement by showing that one element in the domain does not satisfy the predicate. This is called a **counterexample**. 
	
	Statement: All even numbers are divisible by 7. 
	
	Consider the number 16. 16 is an even number, but 16 divided by 7 has a remainder of 2. So 16 is an even number that is not divisible by 7. Therefore, it is not the case that all even numbers are divisible by 7. 

4) For small domains, you can prove a universal statement by showing that it holds for each element in the domain. This is called the **method of exhaustion**. 
	
	Statement: Let {$S = {2, 4, 6}$}. All the numbers in $S$ are even. 
	
	A number is even if it can be written as a product of 2 and another integer. For S, $$2=2*1\;\;\;\;\;\;\;\;4=2*2\;\;\;\;\;\;\;\;6=2*3$$
	
	So the statement is true.