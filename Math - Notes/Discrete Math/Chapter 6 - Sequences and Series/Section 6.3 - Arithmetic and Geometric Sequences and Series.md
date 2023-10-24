# Arithmetic
## Definition
- A **[[Section 6.1 - Sequences#Definition|sequence]] is arithmetic** if it has the form $a_n = dn + c$. A **[[Section 6.2 - Series#Definition|series]] is arithmetic** if it is the sum of an arithmetic sequence.
## Formula
- Let $a_n = dn + c$  be an arithmetic sequence. The sum, $S_k$, of the first $k$ terms of the arithmetic series can be found using the formula: $$S_k = \sum_{n=1}^k a_n = n * \frac{a_1 + a_n}{2}$$
# Geometric
## Definition
- A **sequence is geometric** if it has the form $a_n = a_ir^{n-1}$. A **series is geometric** if it is the sum of a geometric series.
## Formula
- Let $a_n = a_ir^{n-1}$ be a geometric sequence. The sum, $S_k$ , of the first k terms of the geometric series can be found using the formula: $$S_k = \sum_{n=1}^ka_n = a_1 * \frac{(1-r^n)}{(1-r)}$$
# Example - Arithmetic
1) Find the formula for the arithmetic sequence $a_n = 4, 7, 10, 13, 16, ...$ with $n>= 1$.

	Referring back to our [[Section 6.3 - Arithmetic and Geometric Sequences and Series#Definition|definition]] of what an arithmetic sequence is, we know this sequence will go on continuously. We need to use $a_n = dn + c$.

	We need to find what each of the terms are. In order to find $d$, look at how the sequence increments. In our example, the sequence is incrementing by $3$. So, $d=3$. This means: $$a_n = 3(n)+c$$
	In this formula, $c$ is a constant additive. What needs to be added to get our value. Finding $c$ is trivial as we can evaluate $a_1$ and solve for $c$ $$a_1=3(1) + c$$$$4=3+c$$$$c = 1$$
	So our entire formula is:$$a_n = 3(n) + 1$$

2) Find the sum, $S_{100}$ , of the first 100 terms of the sequence using the formula: $$\sum_{n=1}^ka_n = n * \frac{a_1 + a_k}{2}$$
	Breaking down the formula, $n =$ *the number of terms*. Since we are finding the first 100 terms of the sequence, $n=100$. Now we need $a_1$ and $a_2$. $a_1$ is the first term of our sequence, in this case it is $4$.

	$a_2$ on the other hand is going to be the $100^{th}$ term of our sequence. All we need to do it plug $100$ into the formula we found in example 1.
	$$a_{100} = 3(100) + 1$$
	$$a_{100} = 301$$
	Now we have everything we need for the formula. Let's plug everything in.$$\sum_{n=1}^{100}a_{100}=100*\frac{4+301}{2}=15,250$$
# Example - Geometric
1) Find the formula for the geometric sequence $a_n = 8,4,2,1,\frac{1}{2},...$ with $n>= 1$.

Recall that for a geometric sequence, we use the formula:$$a_n=a_1*r^{n-1}$$
$a_1$ is the first term of our sequence, which in this case is $8$. Next we need to find the common ratio, $r$.

First we look at any 2 consecutive terms. In our example we are going from 8 to 4.  We need to take the latter term, $4$, and divide it by the previous term, $8$. This gives us $\frac{1}{2}$. So, $r=\frac{1}{2}$.

Our formula then turns into:$$a_n=8*(\frac{1}{2})^{n-1}$$
And we are done.


2) Find the sum, $S_{100}$, of the first 100 terms of the sequence using the formula:$$S_k=\sum_{n=1}^ka_n=a_1*\frac{(1-r^{n})}{(1-r)}$$
Using the terms we have found above, lets plug everything in.$$S_{100}=8*\frac{(1-\frac{1}{2}^{100})}{(1-\frac{1}{2})}$$
Using a calculator we get $15.999999999999...$ We are just going to round up to $16$. 