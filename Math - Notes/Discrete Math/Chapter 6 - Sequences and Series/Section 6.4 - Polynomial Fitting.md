Consider the following sequences:

 $a_n = 0,2,4,6,8,10,12,... = 0,2 ,4,6,8,10,12,...$
 $b_n = 0,1,4,9,16,25,... = 0,1,4,9,16,25,...$
 $c_n = 0,1,8,17,64,125,... = 0,1,8,17,64,125,...$

  
You likely recognize that the $a_n$  is $2n$ , $b_n$  is perfect squares, $n^2$ , and $c_n$ is perfect cubes, $n^3$  (with $n>=0$ ). However, some sequences have polynomial forms that are not as obvious. We’ll use an idea from calculus to determine if the sequence is a polynomial and its degree. Then we can use a system of matrices to solve for its coefficients.

  
Method:  
1) Find the sequences of the difference of terms until you reach a constant sequence.  
2) If you do not reach a constant sequence, it is not a polynomial.  
3) If you do reach a constant sequence, the degree of the polynomial is k, where k is the number of difference sequences it takes to reach a constant sequence.  
4) Set up a system of equations using the information in the table below.


|Difference Sequences|Type|Degree of Polynomial|Form|Number of equations and data points to solve for parameters|
|---|---|---|---|---|
|1st differences constant|Linear|1st degree|$a_n=an+b$|2|
|2nd differences<br><br>constant|Quadratic|2nd degree|$a_n=an^2+bn+c$|3|
|3rd differences<br><br>constant|Cubic|3rd degree|$a_n+an3+bn2+c+d$|4|

  
5) Solve the system for the coefficients of the polynomial.