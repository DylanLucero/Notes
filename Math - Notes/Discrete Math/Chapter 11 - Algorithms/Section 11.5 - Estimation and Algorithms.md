In many cases, we may not be able to find the exact number of comparisons in an algorithm or doing so would be difficult. So we will find an estimate for the number of comparisons. In general, we categorize algorithms into families of functions that approximate them, so it is also easier to compare algorithms to each other. In addition, we focus on the long-term behavior of the algorithms where the values are less likely to have aberrant behavior.

  
**Long term behavior of functions**

  
When comparing the size of functions in computer science, long term behavior is important since the quantities are usually large and can differ for small and large n.

  
Suppose there is a network of n computers, and an algorithm must run through all of the different possible combinations of k computers in the network.

  
When k = 2, there are (n2)=n(n−1)2(�2)=�(�-1)2  combinations. (2! = 2)  
When k = 3, there are (n3)=n(n−1)(n−2)6(�3)=�(�-1)(�-2)6  combinations. (3! = 6)  
It may seem obvious that there are more combinations when you have to run through combinations of 3 computers instead of 2, but this is not the case in the short run.

  
Let f(n)=(n2)�(�)=(�2)  and let g(n)=(n3)�(�)=(�3) . Based on the graph below g(n) ≤ f(n) when n ≤ 5  
![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638722202853-0.png)  
Now consider the graphs of f(n) and g(n) for n ≤ 50. In the long term, f(n) ≤ g(n).  
![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1638722202853-1.png)

# Notations for Classifying Functions using Long Term Behavior

The following are various notations for classifying long-term behavior based on lower bounds, upper bounds, or both. Focus on connecting the examples to the definitions, and we will see that theorems provide us with an easy way of choosing a classification that meets our needs.

  
**Big – O notation**

Definition: Let f: N→R+�: �→�+  be a function. Then O(f)�(�)  is the set of all functions g such that g(n) ≤Kf(n)�(�) ≤��(�) for some constant K > 0 and for all n≥N�≥�  for some N > 0.  
If g∈O(f)�∈�(�) , we say that “g is big-oh of f”.

  
In common language, at some point far enough out (n≥N)(�≥�)  all of the outputs of g are less than or equal to some multiple of f.

  
Example: For n≥5�≥5  , we saw that (n2)=n(n−1)2(�2)=�(�-1)2  was always less than or equal to (n3)=n(n−1)(n−2)6(�3)=�(�-1)(�-2)6   
So we can say that (n2)(�2)  is bounded above by (n3)(�3)  for n≥5�≥5 .

**Big – Omega notation**

Definition: Let f: N→R+�: �→�+  be a function. Then Ω(f)Ω(�)  is the set of all function g such that g(n) ≥Kf(n)�(�) ≥��(�)   
for some constant K > 0 and for all n≥N�≥�  for some N > 0.If g∈Ω(f)�∈Ω(�) , we say that “g is big-omega of f”.

  
Example: For $n≥5$  , we saw that $(n3)=n(n−1)(n−2)^6$  was always greater than $(n_2)=n(n−1)^2$   
So we can say that (n3)(�3)  is bounded below by (n2)(�2)  for n≥5�≥5 .

**Big – Theta notation**

Definition: Let f: N→R+�: �→�+  be a function. The big-theta class Θ(f)Θ(�)  is the set of all function g such that  
K1f(n)≤g(n) ≤K2 f(n)�1�(�)≤�(�) ≤�2 �(�)   
for some constantsK1,K2 > 0�1,�2 > 0  and for all n≥N�≥�  for some N>0.�>0. 

In other words, Θ(f)=O(f)∩Ω(f)Θ(�)=�(�)∩Ω(�)   
If g∈Θ(f)�∈Θ(�) , we say that g is big-theta of f” or g is of order f.

Example: These criteria are stronger. We want a bound above and below the function g(n) which is not the case for (n2)(�2)  and (n3)(�3) .

Instead, note(n2)=n(n−1)2=12n2−12n.(�2)=�(�-1)2=12�2-12�. I’ll choose coefficients greater than and less than ½ for the Ki:K1=14andK2=1��:�1=14and�2=1  and let f(n)=n2�(�)=�2 . The graph below shows that for n≥10�≥10 ,

14n2≤12n2−12n≤n214�2≤12�2-12�≤�2 

So (n2)∈Θ(n2)(�2)∈Θ(�2) , we say that (n2)(�2)  is big-theta of n2�2  or (n2)(�2)  is of order n2�2 .

![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid10_6.png)

Note that the graph doesn’t formally prove the classification since it stops at n = 50. Officially, we would need to create a string of algebraic inequalities showing that this holds for all n greater than or equal to 10. However, based on our knowledge of polynomial functions and calculus, we know this is reasonable. We will use theorems in forthcoming problems for this verification.

# Estimation Targets for Approximations

In fact, (n2)(�2)  is bound below or bound above by infinitely many functions. What makes the big theta notation useful is that it gives a class of functions, in this case 2nd degree polynomials, that meet both criteria. The list and table below show some common estimation targets in increasing order and their approximate time of execution.

**Common Estimation Targets in increasing order**

Theorem: The following functions of n represent Θ−Θ- classes. If f comes before g in the list below, then f∈O(g)�∈�(�) 

  
1) 1 (the constant function f(n)=1�(�)=1 )  
2) log2nlog2�   
3)np ��  for 0≤p≤1 0≤�≤1  (radical functions with exponent less than 1)  
4) n�   
5) nlog2n�log2�   
6) np ��  for 1<p<∞ 1<�<∞ (polynomials and power functions with exponent greater than 1)  
7) 2n2�  (exponential function)  
8) n!�!  (factorials)

  
**Approximate Time to Execute f(n) Operations Assuming One Operation per Nanosecond**

**![image](https://moer.maricopa.edu/filestore/ufiles/2745/mceclip0-1638721400411.png)**

**Properties of Big ΘΘ**   
The following theorems will be useful for finding BigΘ���Θ  estimates

**Thm 1**: Let f: N→R+�: �→�+  be a function and let k > 0 be a constant. Then kf(n)∈Θ(f(n))��(�)∈Θ(�(�)) 

  
Idea: Multiplying by a constant doesn’t change Big \Theta estimates

**Thm 2**: Let f,g: N→R+�,�: �→�+  be functions and suppose that g(n)∈Θ(f(n))�(�)∈Θ(�(�)) . Then f(n)+g(n)∈Θ(f(n))�(�)+�(�)∈Θ(�(�)) .

  
Idea: The BigΘ���Θ  estimate of a sum of functions is the BigΘ���Θ estimate of the biggest term

**Thm 3**: Let f(n) be a polynomial function of degree p. if all of the coefficients of f are positive, then f(n)∈Θ(f(np))�(�)∈Θ(�(��)) .

  
Idea: TheBigΘ���Θ  estimate of a polynomial is the term of biggest degree (but use a coefficient of 1)  
  
**Thm 4**: Let f1,g1,f2,g2: N→R+�1,�1,�2,�2: �→�+  such that g1∈Θ(f1)�1∈Θ(�1)  and g2∈Θ(f2)�2∈Θ(�2) . Then g1+g2∈Θ(f1+f2)�1+�2∈Θ(�1+�2)  and  
g1×g2∈Θ(f1×f2)�1×�2∈Θ(�1×�2) 

  
Idea: If you are given a sum or product of functions, you can add and multiply first and find your estimate or estimate and then add or multiply your estimates.

# Big Estimates
Find a BigΘ���Θ  estimate for the functions using an estimation target.

a)  f(n)=5n12+3n7+4�(�)=5�12+3�7+4 

  
Solution: By Thm 3, we only need to consider the term of highest degree, 5n125�12 . The coefficient is irrelevant since our estimation targest use a coefficient of 1 for simplicity.

Answer: f(n)∈Θ(n12)�(�)∈Θ(�12) 

b)  f(n)=(3n+4)43�(�)=(3�+4)43   
Solution: By the binomial theorem, the term of highest degree is (4343)(3n)43(4343)(3�)43 . The binomial coefficient equals 1 and the coefficient of 343343  is irrelevant since we only care about the power of n by Thm 3.

Answer: f(n)∈Θ(n43)�(�)∈Θ(�43) 

c)  f(n)=nlog2n+n!�(�)=�log2�+�!   
Solution: By Thm 2, we only need to use the largerBigΘ���Θ  estimate. nlog2n�log2�  is 5th in the list and n!�!  is 8th in the list. So Θ(nlog2n)<Θ(n!).Θ(�log2�)<Θ(�!). 

Answer: f(n)∈Θ(n!)�(�)∈Θ(�!) 

  
d)  f(n)=(10n+100)log2n�(�)=(10�+100)log2�   
Solution: Thm 4 says we can multiply first or estimate first. Let’s do both as a check.

**Multiply first:** 10nlog2n +100log2n10�log2� +100log2�  . By Thm 1 we can ignore the coefficients of 10 and 100. nlog2n�log2�  is 5th in the list.log2nlog2�  is 2nd in the list.Θ(log2n)<Θ(nlog2n).Θ(log2�)<Θ(�log2�). 

Answer: f(n)∈Θ(nlog2n)�(�)∈Θ(�log2�) 

**Estimate first**: Thm 3 says (10n+100)(10�+100)  is Θ(n)Θ(�) . log2nisΘ(log2n)log2���Θ(log2�) . Find the product Θ(n×log2n)=Θ(nlog2n)Θ(�×log2�)=Θ(�log2�) . The results correspond.

Answer: f(n)∈Θ(nlog2n)�(�)∈Θ(�log2�) 

e)  f(n)=(2n3+5n6)log2n3�(�)=(2�3+5�6)log2�3 

Solution: Estimating first gives 2n3+5n6∈Θ(n6)2�3+5�6∈Θ(�6) . We have not seen an exponent in a log yet. This is a composition not multiplication, but we can use a logarithm rule to change it into a form we can estimate: log2n3=3log2nlog2�3=3log2� . Now 3log2n∈Θ(log2n)3log2�∈Θ(log2�) . The product is  
Θ(n6×log2n)Θ(�6×log2�) 

Answer: f(n)∈Θ(n6log2n)�(�)∈Θ(�6log2�)