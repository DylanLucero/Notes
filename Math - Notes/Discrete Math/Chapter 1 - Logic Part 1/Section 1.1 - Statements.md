# Definitions
#### Statement: 
A *statement* or a *proposition* is a sentence which is either true or false but not both.
#### Simple Statement: 
A statement is *simple* (or *atomic*) if it cannot be divided into smaller statements, otherwise it is called a *compound statement*
#### Compound Statement: 
A compound statement is a statement that is composed of two or more atomic statements.

## Example Statements
1. A cat is a mammal.
2. It is raining.
3. You will work hard in this course.
4. Pigs can fly.

Notice each statement is a complete sentence with a noun and a verb. Each statement also has a *truth value*, a designation of whether the statement is true of false. We may not know this truth value, but each statement does have a single truth value.

## Example Not-Statements
1. The blue hat.
2. A number between 0 and 1.
3. Patriotic Americans.

Notice that each of these phrases are not statements. They are not sentences and you cannot determine a truth value for them.

# Logical Symbols
(also called logical connectives)
Logical symbols are used to create more complex statements.

Let p and q be simple statements.

1. The *negation of p* is denoted ~p. It is read as "Not p" or "It is not the case that p". (Logical NOT)
2. The *conjunction of p and q* is denoted  p ^ q. It is read as "p and q".  (Logical AND)
3. The disjunction of p and q is denoted p v q. It is read as "p or q". (Logical OR)

We do follow a certain order of operations, generally if there are more than one symbol in a compound statement, **negation** is performed first and **parenthesis** are used to indicate the intended order.

# Truth Tables
#### Definition
A **truth table** is an enumeration of all the possible truth values of the simple statements that comprise a compound statements and the resulting truth values of the compound statements.

#### Truth Table for Negation of p
A simple statement p can only have one or two truth values: true or false. The negation of p, ~p, has the opposite truth value of p.

| p | ~p |
| :--: | :--: |
|T |  F |
| F | T |

#### Truth Table for the Conjunction of p and q
The simple statements p and q can only have one of two truth values: true or false. However, combined there are 4 truth value possibilities. The conjunction of p and q, p ^ q, is only true when p is true *and* q is true. Otherwise, the compound statement is false.

|p|q|p^q|
|:--:|:--:|:--:|
|T|T|T|
|T|F|F|
|F|T|F|
|F|F|F|

#### Truth Table for the Disjunction of p and q
The truth table for the disjunction of p and q is like the conjunction. However, the disjunction of p and q, p v q, is only false when p is false *and* q is false. Otherwise, the compound statement is true.

|p|q|p v q|
|:--:|:--:|:--:|
|T|T|T|
|T|F|T|
|F|F|F|