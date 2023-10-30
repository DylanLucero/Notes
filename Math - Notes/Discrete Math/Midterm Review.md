# Chapter 1
1. Use the statements defined below to write the sentences in symbolic form.
	Let p = Scar is king
	Let q = There is food in the Pridelands
	Let r = Simba is home

a) If Scar is king then Simba is not home and there is no food in the Pridelands.

b) If Simba is home or there is food in the pride lands then scar is not king

c) Simba is home but there is no food in the Pridelands.

d) Simba is home or scar is king

a) if p then not r and not q 
	p->$\neg$ r ^ $\neg$ q
b) if r or q then not p
	r v q -> $\neg$ p
c)r and not q
	r ^ $\neg$q
d)r or q
	r v q

---
2. Construct the truth table for (p ∧ ¬q) =⇒ (r ∨ q). Use the standard
set up for the truth table shown in the videos.

|  p  |  q  |  r  | $\neg q$ | ($p \land \neg q$) | ($r \lor q$) | ($p \land \neg q -> (r \lor q)$ ) |
|:---:|:---:|:---:|:--------:|:------------------:|:------------:| :---------------------------------: |
|  1  |  1  |  1  |    0     |         F          |      T       |              T                     |
|  1  |  1  |  0  |    0     |         F          |      T       |               T                    |
|  1  |  0  |  1  |    1     |         T          |      T       |                T                   |
|  1  |  0  |  0  |    1     |         T          |      F       |                 F                  |
|  0  |  1  |  1  |    0     |         F          |      T       |                  T                 |
|  0  |  1  |  0  |    0     |         F          |      T       |                   T                |
|  0  |  0  |  1  |    1     |         F          |      T       |                    T               |
|  0  |  0  |  0  |    1     |         F          |      F       |                     T              |

3. Use truth tables to determine if the statements below are logically equiv-
alent. Justify your answer. Use the standard set up for truth tables shown in
the videos.

Statement 1: ¬(p ∧ ¬q) =⇒ r
Statement 2: ¬r =⇒ ¬(p =⇒ q)

| $p$ | $\neg p$ | $q$ | $\neg q$ | $r$ | $\neg r$ | $\neg(p \land \neg q)$ | $\neg(p \land \neg q)$ -> $r$ | $p$ -> $q$ | $\neg (p \land q)$ | $\neg(p \land \neg q)$ -> $r$ $\equiv ¬r$ $¬(p$ -> $q)$ |
| --- | -------- | --- | -------- | --- | -------- | ---------------------- | ----------------------------- | ---------- | ------------------ | ------------------------------------------------------- |
|     |          |     |          |     |          |                        |                               |            |                    |                                                         |

---
4. Define the simple statement p and q as follows:
	p=$5<x$
	q=$x≤9$

	a) Rewrite the compound statement 5 < x ≤ 9 in logic form using p and q
		$p \land q$
	b) Write the negation of the statement symbolically and apply DeMorgan’s Law to remove the parentheses
	
	c) Translate the negation of the symbolic form into English (you may use math
	symbols as well, but no logic symbols)

---
# Chapter 2
1. Consider the universal statement, “All perfect squares are divisible by its square root.”
Let the domain D = The set of perfect squares and P (x) = x is divisible by $\sqrt x$ where x ∈ D.

a) Write the statement symbolically
	$\forall x \in D(P(x))$
b) Write the negation symbolically
	$\exists x \in D(\neg P(x))$
c) Write the negation in words.
	There exists an element in the set D where x is not divisible by $\sqrt x$.

---
2. Consider the existential statement, “Some multiples of 5 are even.”

Let the domain D = the set of multiples of 5 and P (x) = “x is even” where x ∈ D.

a) Write the statement symbolically
	$\exists x \in D,P(x)$
b) Write the negation symbolically
	$\forall x \in D,(\neg P(x))$
c) Write the negation in words.
	For all elements in D, x is not even.

---
3. Consider the universal statement, “All multiples of 8 are multiples of 4.” 

Using the domain of integers, write the universal statement as a conditional statement in words.

For all integers $n$, if $n$ is a multiple of 8, $n$ is a multiple of 4.

---
4. Consider the existential statement, “There exists a perfect square that is even.” Using the domain of integers, write the existential statement as a conjunction statement in words.

 There exists an $n$ that is a perfect square and is even. 

---
5. Write the negation of the following statements. (Use the negation rules for Universal and Existential Statements in [[Section 2.4 - Equivalent Forms of Quantified Statements|Section 2.4]].)

a) For all integers n, if $n^2$ is even, then n is even.
	There exists an integer, $n$, such that $n^2$ is even and $n$ is odd.

b) For all integers x and y, if x or y is even, then the product xy is even. (Note:
Use DeMorgans Law.)
	There exists integers x and y such that x or y is even and the product, xy, is odd.

c) There exists a real number x such that x < 1 and $x^2$ > 1.
	For all real numbers, x, x < 1 or $x^{2}> 1$

---
6. Provide a direct proof: Let a, b, c be integers. If a|b and a|c then a|(b ∗ c).
	