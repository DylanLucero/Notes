# Connecting Permutations and Indistinguishable Permutations

Definition: A counting problem involves _**indistinguishable permutations**_ when two or more elements of the set we are permuting are identical or indistinguishable and we account for the reduction for the number of outcomes.

Recall that if we have three letters, A, B, and C, the total number of permutations is  3! = 6. The list of permutations is enumerated below.

  
List of Permutations: ABC, ACB, BAC, BCA, CAB, CBA

  
Now suppose the three letters we are permuting are A, A, and B. In particular, we may have A listed twice in a permutation, but we cannot distinguish between the A’s.

  
Let’s first pretend we could tell the A’s apart. We will call them $A_1$ and $A_2$. I used the permutations of A, B, and C and replaced A with $A_1$ and C with $A_2$. The permutations are enumerated below.

  
List of Permutations: $A_1BA_2, A_1A_2B, BA_1A_2, BA_2A_1, A_2A_1B, A_2BA_1$
  
The table below shows these permutations and their corresponding permutations with the subscripts for A. Note the $1^{st}$ and $6^{th}$ are both ABA, the $2^{nd}$ and $5^{th}$ are both AAB, and the $3^{rd}$ and $4^{th}$ are both BAA.

|$A_1BA_2$|$A_1A_2B$|$BA_1A_2$|$BA_2A_1$|$A_2A_1B$|$A_2BA_1$|
|---|---|---|---|---|---|
|$ABA$|$AAB$|$BAA$|$BAA$|$AAB$|$ABA$|

So the corresponding indistinguishable permutations are ABA, AAB, and BAA for a total of 3.

To count the indistinguishable permutations from the original permutations, we divide by the number of ways to arrange the A’s if they were indistinguishable or $$\frac{3!}{2!}= \frac{{3×2×1}}{{2×1}}=3$$
### Formula
The number of indistinguishable permutations of n objects where there are $r_i$  of indistinguishable type $i$ for $1≤i≤k$ is

 $$\frac{n!}{r_1!\; r_2!\; ×\;...×\;r_k!}$$
# Indistinguishable Permutations
a) Find the number of indistinguishable permutations of the letters in MISSISSIPPI

  
Solution: MISSISSIPPI has 11 letters.

Number of M’s = 1  
Number of I’s = 4  
Number of S’s = 4  
Number of P’s = 2

So $n=11,\;r_1=1,\;r_2=4,\;r_3=4,\;r_4=2,\;k=4$
 $$\frac{n!}{r1! r2!×...×rk!}=\frac{11!}{1!\;4!\;4!\;2!}$$
$$=\frac{39,916,800}{1×24×24×2}=34,650$$

#### Note 
If all of the letters are distinguishable, we would divide by a bunch of 1! which corresponds to the original permutation formula.

b) How many 16-bit strings containing only 0’s and 1’s have 7 1’s?

Solution:

Number of bits: 16  
Number of 1’s: 7  
Number of 0’s: 9
$$\frac{16!}{7!\;9!}=11,440$$

c) How many 8 letter strings containing only a’s, b’s, and c’s have 3 a’s and 2 b’s?

Solution:
Number of letters: 8  
Number of a’s: 3  
Number of b’s: 2  
Number of c’s: 3  
$$\frac{8!}{3!2!3!}=560$$