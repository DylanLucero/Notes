# Definitions
Logical Equivalence:
Two statements are *logically equivalent* if and only if they have identical truth values for all possible combinations of their truth values. ^44aa4e

Tautology: 
a *tautology* is a statement that is true for all possible combinations of truth values. ^463978

Contradiction: 
A *contradiction* is a statement that is false for all possible combinations of truth values. ^6e5003

# Guidelines for justifying whether two statements are logically equivalent
- Create the [[Section 1.1 - Statements#Truth Tables|truth tables]] for the two statements.

- Determine whether the truth values for the statements are identical.

- Make one of the following statements for the justification

	- [[Section 1.2 - Logical Equivalence#^44aa4e|Logically Equivalent]]: Since columns X and Y have identical truth values for all possible combinations of (list atomic statements), the statements are logically equivalent.
	
	- **Not Logically Equivalent**: Since columns X and Y do not have identical truth values in rows (list the rows), the statements are not logically equivalent.

# Guidelines for justifying whether a statement is a tautology, contradiction or neither

- Create a truth table for the statement.

- Determine whether the column for the statement is all T, all F, or some T and some F.

- Make one of the following statements for the justification: 
	- a) Since the truth values for the statement are all true, the statement is a tautology. 
	- b) Since the truth values for the statement are all false, the statement is a contradiction. 
	- c) Since the truth values for the statement contain both true values and false values, the statement is neither a tautology or a contradiction.

# DeMorgan's Law
DeMorgan's Law is the negation of conjunctions and disjunctions.

1. The negation of the conjunction p ^ q is ~ (p ^ q). DeMorgan's Law states that ~(p^q) is logically equivalent to ~p v ~q.

2. The negation of the disjunction, p v q , is ~(p v q). DeMorgan's Law states that ~(p v q) is logically equivalent to ~p ^ ~q.