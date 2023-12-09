A **_permutation_** is an ordered arrangement of the elements of a set. 


There are three people that are taking turns using the swing on a playground: Amy, Beth, and Carl. List all the different orders in which they can use the swing where everyone gets exactly one turn. How many different ways are there?


Solution: First we will list all of the ways. We will abbreviate the names by using the letters A, B, and C. It is important to use a systematic method, so you don’t miss any possible arrangements. We will start by writing all the arrangements with A first, then B, and then C.


First Letter A: ABC, ACB  
First Letter B: BAC, BCA  
First Letter C: CAB, CBA


Answer: List of Permutations: ABC, ACB, BAC, BCA, CAB, CBA  
Number of Permutations: 6


Counting Permutations Directly: Making a list of permutations can be tedious when there are more than 3 objects to permute. To count the number of possible permutations without making a list, we can use a variation on the Fundamental Counting Principle.


One difference between the fundamental counting principle and permutations, is that with permutations our choices are dependent. We begin with one group of objects, and with every choice we make, we have one less option to choose from for our next choice.

  
One similarity between the fundamental counting principle and permutations, is that we will require that there is a sequence or order to our choices. What this means is that each choice corresponds to one specific outcome.

# Permutations and Counting
a) There are three people that are taking turns using the swing on a playground: Amy, Beth, and Carl. How many different ways are there in which they can use the swing where everyone gets exactly one turn?

Solution: This problem is identical to problem 7, but we will solve it using multiplication. There are 3 options for who goes first. There are 2 remaining options for who goes second after we choose the first person. And there is only one option for who goes third (only one person remains). So the number of ways is

$$3×2×1=6 $$
Answer: 6

  
b) Don has 12 books on his summer reading list. He wants to choose 4 books to read in order from first to last. In how many ways can he do this?

  
Solution: Observe that there are a total of 12 books, 4 are to be chosen, and the order in which he reads them matters. Sometimes it can be helpful to make a diagram to set up your multiplication as shown below.

  
![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid20_1.png)

$$12×11×10×9=11,880$$

Answer: 11,880 ways

# Formula for Permutations 
You are given a group of $n$ objects and want to select $r$ of the objects where the order of the objects matters. The number of such permutations is the product of $r$ factors, beginning at n, and decreasing by $1$ for each successive factor.

## Notation 
$nPr=n×(n−1)×(n−2)×...(n−r+1)$

Or equivalently, $nPr= \frac{n!}{(n−r)!}$ 

### Note 
In part $a, n = r$ (both 3). This is called a factorial denoted, $3!$, read “3 factorial”.

### Definition
$n!$ (read “n factorial”) is the product of all of the natural numbers from n to 1.  
$$n!=n×(n−1)×(n−2)×...3×2×1$$
# Permutations
a) The student council has 14 students. They need to choose a President, Vice President, Secretary and Treasurer for student council. In how many ways can the 4 different positions be appointed from the 14 students?

$$\frac{14}{P}*\frac{13}{VP}*\frac{12}{S}*\frac{11}{T} = 24,024$$

Can also be written as, $$_{14}P_4$$
and, $$\frac{n!}{(n-r)!}=\frac{14!}{(14-4)!}=\frac{14!}{10!}=\frac{14*13*12*...*2*1}{10*9*8*...*2*1} = 14*13*12*11$$



b) James is creating a 5-digit passcode using the digits 0 through 9. How many 5-digit passcodes are possible if the numbers cannot be repeated?

$$\frac{10}{1^{st}}*\frac{9}{2^{nd}}*\frac{8}{3^{rd}}*\frac{7}{4^{th}}*\frac{6}{5^{th}} =30,240$$
Can also be written as,$$_{10}P_5$$
and,
$$\frac{n!}{(n-r)!}=\frac{10!}{(10-5)!}=\frac{10!}{5!}=10*9*8*7*6$$



c) Three cards are chosen without replacement from a deck of 52 cards and placed in order from first to third. How many outcomes are possible?
$$\frac{52}{1^{st}}*\frac{51}{2^{nd}}*\frac{50}{3^{rd}} = 132,600$$
can also be written as,$$_{52}P_3$$

# Permutations with Variations
Five cards are chosen without replacement from a deck of 52 cards and placed in order from first to fifth.
  
a) If the first card must be a King, how many outcomes are possible?
$$\frac{4}{1^{st}}*\frac{51}{2^{nd}} * \frac{50}{3^{rd}} * \frac{49}{4^{th}} * \frac{48}{5^{th}}=23,990,400$$or,$$_4P_1$$
b) How many outcomes contain all clubs?
$$\frac{13}{1^{st}} * \frac{12}{2^{nd}} * \frac{11}{3^{rd}} * \frac{10}{4^{th}} * \frac{9}{5^{th}}=154,440$$
  
c) How many outcomes contain at least 1 Diamond?

We are going to do the total number of outcomes - the outcomes with no diamonds

Without diamonds,$$39*38*37*36*35 = 69,090,840$$
Total Number of outcomes,$$52*51*50*49*48=311,875,200$$
Now we subtract,$$311,875,200-69,090,840=242,784,360$$
![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1636616901150-0.png)