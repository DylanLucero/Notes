# Arithmetic Sequences

A **sequence is arithmetic** if it has the form $a_{n}= dn +c$

## Example

Let $a_{n}= 3n+4$ for 

| n     | 1   | 2   | 3   | 4   | 5   | 6   |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| $a_n$ | 7   | 10  | 13  | 16  | 19  | 22  | 

| $\Delta a_n$ | $+3$     | +3        | +3        | +3        | +3  |
| :--: | :--: | :--: | :--: | :--: | :--: |
|              | $7+3=10$ | $10+3=13$ | $13+3=16$ | $16+3=19$ | $19+3=22$    |

**Pattern**: In general, the next term equals the previous term plus 4 and the initial term is 7.

**Recursive Form**: $a_{n+1}=a_{n}+3$. Initial condition: $a_{1}=7$

**Formula**: An arithmetic sequence of the form $a_{n}=dn+c$ can be written in recursive form with $$a_{1}=d(1)+c\;and\;a_{n}=a_{n-1}+d$$
**Note**: I used an index of 1 for the initial value of the sequence. It changes slightly for an initial value of $n=0$.

# Geometric Sequences
A **sequence is geometric** if it has the form $a_n=a_{1}r^{n-1}$
## Example
Let $a_n=2(3)^n$ for $n \geq 0$

| n     | 0   | 1   | 2   | 3   | 4   | 5   |
| ----- | --- | --- | --- | --- | --- | --- |
| $a_n$ | 2   | 6   | 18  | 54  | 162 | 486 | 

| $\frac{a_{1}+1}{a_n}$ |        +3        |        +3         |         +3         | +3  | +3  |
|:---------------------:|:----------------:|:-----------------:|:------------------:|:---:|:---:|
||    $\frac{6}{2}=3$    | $\frac{18}{6}=3$ | $\frac{54}{18}=3$ | $\frac{162}{54}=3$ | $\frac{3486}{162}= 3$    |     

**Pattern**: In general, the next term equals the previous term times 3 and the initial term is 2.

**Recursive Form**: $a_n=3a_{n-1}$ for $n \geq 1$. Initial condition: $a_{0}=2$.

**Formula**: A geometric sequence of the form $a_n=br^n$ can be written in recursive form with $a_{0}=b\;and\;a_{n}=b \times a_n=1$ .

*Note:* I used an index of - for the initial value of the sequence. It changes slightly for an initial value of $n=1$.