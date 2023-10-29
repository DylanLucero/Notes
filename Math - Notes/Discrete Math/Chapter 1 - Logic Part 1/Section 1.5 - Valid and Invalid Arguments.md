# Definition

An ***argument*** is a sequence of statements composed of one or more premises and a single conclusion.

An argument is **valid** if assuming all the premises to be true yields that the conclusion is true. Otherwise, an argument is **invalid**.

Here are two examples of arguments. We always write the premises first, each on a single line. The conclusion is written last and is preceded by the therefore symbol denoted by “∴”.

1. If p then q (premise 1)
	p                   (premise 2)
	∴ q               (conclusion)

2. p v q    (premise 1)
	p -> r   (premise 2)
	q -> r   (premise 3)
	∴ r         (conclusion)

# Guidelines for justifying whether an argument is valid or invalid
- Create a truth table containing all the premises and the conclusion.

- Determine any rows where all of the premises are true.

- Determine if the conclusion is also true in these rows.

- If the conclusion is true whenever all the premises are true, the argument is valid

- If the conclusion is false for one or more cases where the premises are all true, the argument is invalid.

- Justify your decision using one of the following statements:
	- The premises are all true in rows(list rows). The conclusion is also true in these rows. Therefore, this is a valid argument.
	
	- The premises are all true in rows(list rows). However, the conclusion is false in rows(list rows). Therefore, this is an invalid argument.

# Reference table for some common rules of inference

1) Modus Ponens: 
	p → q 
	p 
	∴ q 
2) Modus Tollens:
	p → q
	 ~q 
	 ∴ ~p 
3) Generalization:
	 p                           q 
	∴ p ˅ q                  ∴ p ˅ q 
4) Specialization:
	p ˄ q                      p ˄ q 
	∴ p                         ∴ q 
5) Conjunction:
	p
	q 
	∴ p ˄ q 
6) Elimination:
	p ˅ q                      p ˅ q 
	~p                          ~q 
	∴ q                         ∴ p 
7) Transitivity:
	 p → q 
	 q → r 
	 ∴p → r 
8) Division into Cases:
	 p ˅ q 
	 p → r 
	 q → r 
	 ∴ r 
9) Contradiction:
	~p → c 
	∴ p