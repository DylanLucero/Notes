The _**fundamental counting principle or multiplication rule**_, in its simplest form, states that if you have two independent choices to make, and the first choice has $m_1$ options and the second choice has $m_2$  options, there are $m_1×m_2$  total ways to make these two choices.

**Extension of Fundamental Counting Principle**: This idea extends to more than 2 choices as follows. If you have n choices to make and $m_j$  options for the $j^{th}$  choice, $1≤j≤n$, the total number of ways to make the $n$ choices is

$$m_1×m_2× ... ×m_n$$

In simpler terms, for any whole number of independent choices you need to make, you can multiply the number of options for each choice to find the total number of possibilities for all the choices.

# Fundamental Counting Principle
a) Suppose you are having lunch at a pizza parlor, and they have a lunch special where you can purchase a slice and a soda. The options for the choices of slice and soda are given below.  How many different slice and soda pairings are possible?  Use a table to enumerate the possibilities.

Slice Options:  Cheese, Pepperoni, White, Veggie, Sicilian, Meat, Hawaiian

Soda Options:  Cola, Diet Cola, Lemon-lime, Seltzer

Solution:  We can make a list of the options in a table as shown below.

|            | Cheese(Ch) | Pepperoni(P) | White(W) | Veggie(V) | Sicilian(S) | Meat(M) | Hawaiian(H) |     
| ---------- | ---------- | ------------ | -------- | --------- | ----------- | ------- | ----------- | 
| Cola (C)   | Ch/C       | P/C          | W/C      | V/C       | S/C         | M/C     | H/C         |     
| Diet (D)   | Ch/D       | P/D          | W/D      | V/D       | S/D         | M/D     | H/D         |     
| Lemon(L)   | Ch/L       | P/L          | W/L      | V/L       | S/L         | M/L     | H/L         |     
| Seltzer(S) | Ch/S       | P/S          | W/S      | V/S       | S/S         | M/S     | H/S         |     

If we count the pairings, we can see there are a total of 28.  Moreover, based on the fundamental counting principle, there are 7 options for the pizza choice, and 4 options for the soda choice.  Therefore, there are $7 × 4 =28$ total options.  This corresponds to the 4 rows and $7$ columns of the table creating $7 × 4 = 28$ cells each with a different pairing.

Answer:  There are $28$ different pairings.

b) You need to select a password that meets the following criteria:

- The first symbol must be a digit less than $4$. 
- The second symbol must be from the set {!, &, %}
- The third symbol must be a vowel

How many possible passwords are there?

Solution:  There are 4 options for the first choice, 3 options for the second choice, and 5 options for the third choice.

Number of possible passwords = $4×3×5=60$ 

c) A license plate is three letters followed by four digits. How many license plates are possible?

Solution:  There are 26 letters in the alphabet and 10 digits (remember to include 0).  So there are 26 options for each of the three letter choices and 10 options for each of the four-digit choices.  By the fundamental principle of counting,

Total number of options = $26^3×10^4=175,760,000$