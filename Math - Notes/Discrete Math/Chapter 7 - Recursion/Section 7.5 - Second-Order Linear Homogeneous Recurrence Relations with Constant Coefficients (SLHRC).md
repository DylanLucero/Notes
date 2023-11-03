# Second-Order Linear Homogeneous Recurrence Relation with Constant Coefficients
A **Second-Order Linear Homogeneous Recurrence Relation with Constant Coefficients** has the form $a_k=Aa_{k-1}+Ba_{k-2}$ for all integers $k$ that are greater than some integer where A and B are real numbers and $B\not= 0$.

**Second Order**: There are two previous terms, namely, $a_{k-1}, a_{k-2}$

**Linear**:$a_{k-1}, a_{k-2}$ are separate terms raised to the first power.

**Homogeneous**: $a_{k-1}, a_{k-2}$ are raised to the same power (1) and there are no other terms of a different power such as a constant added to the sequence.

**Constant Coefficients**: A and B are real fixed numbers and do not depend on $k$.

**Examples that do not meet criteria!**

$a_{k}=2a_{k-1}+3a_k-2+4a_{k-3}$     Three previous terms so not second order
$a_k=2a_{k-1}+a^{2}_{k-2}$     The second term is squared so not linear
$a_k=2a_{k-1}+ 3a_{k-2}+5$     The constant 5 is not linear so not homogeneous
$a_k=ka_{k-1}+3a_{k-2}$     The first term has a factor of $k$ which is not a constant coefficient

**Definition**: Let $a_k=Aa_{k-1}+Ba_{k-2},$ for all integers $k\geq2$ with $B\not=0$. We define the *characteristic equation of the relation as $t^2-At-B=0$

## Example
#### Finding a characteristic equation and its solutions

Let $a_k=a_{k-1}+2a_{k-2}$ for all integers $k\geq2$. Find the characteristic equation of $a_{k}$ and its solutions.

Observe that $A=1$ and $B=2$. So the characteristic equation of $a_K$ is$$t^2-1t-2=0$$
Factoring and solving for $t$ yields $(t-2)(t+1)=0$ and $t=2,-1$

#### Finding the coefficients based on initial conditions

Let $a_k=a_{k-1}+2a_{k-2}$ for all integers $k\geq2$ with $a_0=1$ and $a_{1}= 8$. Find C and D such that:$$\begin{array}{arr}a_{0}=C\times2^0+D\times(-1)^0\\a_1=C\times2^1+D\times(-1)^1 \end{array}$$
$a_{0}= 1$ and $a_1=8$, so replace these values in the equations and simplify
$$\begin{array}{arr}1=C\times1+D\times1\\8=C\times2+D\times-1 \end{array}$$
So our system of equations as a matrix is $$\left[\begin{array}{ccc}
1 &&1&&1\\2&&-1&&8\end{array}\right]$$
Solve using your favorite methods (I used a calc) and the Reverse Row Echelon is
$$\left[\begin{array}{ccc}1&&0&&3\\0&&1&&-2\end{array}\right]$$
So, the sequence that meets the initial conditions is
$a_n=3(2)^n-2(1)^n$ for integers $n\geq0$
