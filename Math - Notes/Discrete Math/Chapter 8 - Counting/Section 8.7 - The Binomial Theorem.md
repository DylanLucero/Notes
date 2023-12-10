
The _**binomial theorem**_ states that for any real numbers a, b, and non-negative integer n,

$$(a+b)^n=\sum\limits^n_{k=0}\begin{pmatrix}n\\k\end{pmatrix}a^{n−k}b^k$$
# Expanding using the Binomial Theorem 
Expand the binomial $(x+3)^7$ using the binomial theorem.  
$$a=x\;\;\;\;\;b=3\;\;\;\;\;n=7$$
$$\begin{pmatrix}7\\0\end{pmatrix}x^{7-0}*3^0+\begin{pmatrix}7\\1\end{pmatrix}x^{7-1}*3^1+\begin{pmatrix}7\\2\end{pmatrix}x^{7-2}*3^2+\begin{pmatrix}7\\3\end{pmatrix}x^{7-3}*3^3+\begin{pmatrix}7\\4\end{pmatrix}x^{7-4}*3^4+
$$$$\begin{pmatrix}7\\5\end{pmatrix}x^{7-5}*3^5+\begin{pmatrix}7\\6\end{pmatrix}x^{7-6}*3^6+\begin{pmatrix}7\\7\end{pmatrix}x^{7-7}*3^7$$
**Remember, $\begin{pmatrix}n\\k\end{pmatrix}$ corresponds to the $n^{th}$ row and $k^{th}$ column of [[Section 7.4 - Pascal’s Triangle|Pascal's Triangle]].**
$$(1x^{7}*1)+(7x^6*3)+(21x^5*9)+(35x^4*27)+(35x^3*81)+(21x^2*243)+$$
$$(7x^1*729)+(1x^0*2187)$$
Simplifying results in,$$x^7+21x^6+189x^5+945x^4+2835x^3+5103x^2+5103x+2187$$
# Simplify using the Binomial Theorem
Write the following in closed form (no summation symbol) using the binomial theorem.

$$\sum\limits^n_{k=0}\begin{pmatrix}n\\k\end{pmatrix}9^k$$
Recall that the Binomial Theorem is $$(a+b)^n=\sum\limits^n_{k=0}\begin{pmatrix}n\\k\end{pmatrix}a^{n−k}b^k$$
Using this form, we can start labeling a, b, and n. Since $9$ is raised to the $k$, this is our $b$.
So,$$b=9\;\;\;\;\;n=n$$
We can think of $a$ to be $(1)^{n-k}$ since 1 times anything it itself.
So, $$a=1\;\;\;\;\;b=9\;\;\;\;\;n=n$$
Which makes our closed form expression $$(1+9)^n=10^n$$