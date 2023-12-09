A _**combination**_ is an unordered selection of a set of objects.
  
**Note** 
With Permutations we say “arrangements” and with combinations we say “selection”.
  
Like permutations, combinations are chosen from a single group of objects. In addition, combinations do not allow for repetition since the items are chosen without replacement, and therefore, each choice is dependent on a previous choice. However, recall that permutations distinguished between the sequence or order of its objects, but combinations do not. This lack of ordering in combinations is the essential difference between permutations and combinations.

For instance, with permutations, 123 and 321 are considered different possibilities or outcomes just as the numbers one hundred twenty-three and three hundred twenty-one are different. With combinations, our result is a subset of the original set of objects and our only concern is what objects were chosen or not chosen. So with combinations, 123 and 321 are not different because they both contain the same three numbers. This may remind you of our study of sets. The sets {1, 2, 3} and {3, 2, 1} are equal since they contain the same elements. Their ordering within the set brackets is irrelevant.

# From Permutations to Combinations
There are 8 kids on the playground that want a turn using the swing: Amy, Beth, Carl, Dan, Ed, Fin, Greg, and Hope. However, there is only enough time for 3 kids to have a turn before the playground closes.

a) How many ways are there to choose 3 of the 8 children to get the 1st, 2nd, and 3rd turn on the swing?

Solution: Observe that this problem asks how to choose an ordering of three of the eight children. So this is a permutation with the group being the 8 children, and 3 children chosen to be first, second and third.  
1st child on swing: 8 options, 2nd child on swing: 7 options, 3rd child on swing: 6 options

$$_8P_{3}=\frac{8!}{(8−3)!}=\frac{8!}{5!}$$
$$8×7×6=336$$
Answer: There are 336 ways to choose 3 of the 8 children to go 1st, 2nd, and 3rd.


b) Now suppose we do not care what order the children get to use the swing. We just want to know all the ways that we can choose 3 of the 8 children to get a turn on the swing. How many ways can we choose 3 of the 8 children?

  
Solution: This is the number of combinations of 3 children being chosen from a group of 8 since the ordering of the children on the swing does not matter. Let’s use this opportunity to adapt the permutation formula to find the number of combinations.

  
Recall from Problem 7, we counted the number of ways three children could each take a turn using the swing in order. We abbreviated the names Amy, Beth, and Carl, by using the letters A, B, and C, and found the following six permutations.

  
List of Permutations: ABC, ACB, BAC, BCA, CAB, CBA

  
We noted that this could be found directly by computing

$$_3P_3=3×2×1=6$$

and that an alternative notation when the number of objects equals the number of choices in a permutation is called a factorial, and denoted 3!.

  
For combinations, all six of these permutations would be considered one possible combination, namely the set {A, B, C}. Observe that any possible combination of three elements has 3! corresponding permutations. Therefore, to find the number of combinations, we can divide the number of permutations by 3!.


Number of Combinations $$\frac{_8P_3}{3!}=\frac{8×7×6}{3×2×1}=\frac{336}{6}=56$$ 
# Formula for Combinations
You are given a group of n objects and want to select r of the objects where the order of the objects does not matter. The number of such combinations is the product of r factors, beginning at n, and decreasing by 1 for each successive factor, divided by r factorial.

$$\left(\begin{array}{arr} n \\ r\end{array}\right)=nCr=\frac{_nP_r}{r!}$$
Or equivalently,$$\left(\begin{array}{arr} n \\ r\end{array}\right)=nCr=\frac{n!}{(n−r)!*r!}$$
# Combinations
a) A committee has 13 members. Four members must be chosen for a subcommittee. In how many ways can the 4 members be chosen for a subcommittee from the 13 members?

$$\left(\begin{array}{arr} 13\\4\end{array}\right)=_{13}C_r=\frac{13!}{(13-4)!*4!}=\frac{13!}{9!*4!}=\frac{13*12*11*10}{4*3*2*1}=\frac{13*11*10}{2}=\frac{1430}{2}=715$$


b) A committee has 13 members. Four members must be chosen for a subcommittee. Three of the 13 members are from the human resources department. If the subcommittee must have exactly one member from human resources, how many four member subcommittees are possible?

$$_3C_{1}\;* \;_{10}C_{3}=\frac{3!}{1!}* \frac{10!}{3!}=\frac{{3*10*9*8}}{{3*2*1*1}}= \frac{{10*9*4}}{1}=360$$
  
c) A committee has 13 members. Four members must be chosen for a subcommittee. Four of the 13 members are from the IT department. If the subcommittee must have at least 1 person from IT, how many four member subcommittees are possible?

Since we are finding subcommitees with at least 1 person from IT, we can take the total number of committees, which is 715 (found in part a) - the number of committees with at least 0 person in IT. 

Finding the amount of committees with 0 people in IT,
$$\frac{9*8*7*6}{4!}= \frac{9*8*7*6}{4*3*2*1}=\frac{9*8*7}{4}=126$$
Now we subtract, $$715-126=589$$
# Combinations with Variations
A poker hand has 5 cards, and the order of the cards does not matter.  
a) How many 5 card poker hands are there?

  
b) A flush is a 5-card poker hand where all the cards have the same suit. How many 5 cards poker hands are a flush that is all clubs?

  
c) How many 5 card poker hands are a flush of any suit?

  
d) A four of a kind is a 5-card poker hand where 4 of the cards have the same rank (A, 2, 3 …) and one other card called the “kicker”. How many ways are there of drawing a four of a kind with four aces and any other card as a kicker?