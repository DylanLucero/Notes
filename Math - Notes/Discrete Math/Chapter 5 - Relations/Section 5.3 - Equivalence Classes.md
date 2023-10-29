# Definitions

Partition: 
A ***partition*** of a set A is a finite or infinite collection of subsets, $P_1, P_2, ...$ where the intersection of **any** two subsets is empty, $P_i \cap P_j = \varnothing, \forall i,j$ and the union of all subsets equals the set $A = P_1 \cup P_2 \cup ...$. ^82b94b

# Example 
**Problem 10 Worked Example – Partition of a Two Set Venn Diagram**:

In chapter 3, we found a partition of a two set Venn Diagram to aid in our counting of elements. We will define it here more formally. 
Let A and B be sets with $A,B \subseteq U$ 
Define P as follows: 

Let $x \in U$ 
	$x \in P_1$, if $x \in A$ and $x \notin B$ 
	$x \in P_2$, if $x \in A$ and $x \in B$
	$x \in P_3$, if $x \notin A$ and $x \in B$
	$x \in P_4$, if $x \notin A$ and $x \notin B$
	
P is a partition of U because: 
1) The intersection of any two partition blocks is empty (mutually disjoint). 
2) The union of all 4 partition blocks equals the set U. 

>Fact: Let U be a set with partition P. Let R be a relation induced by partition P. Then R is reflexive, symmetric, and transitive, and therefore R is an equivalence relation.

Equivalence Class: Let A be a set with R an equivalence relation on A. For any element $a \in A$ the **equivalence class** of a, denoted [a], is the set of all elements in A such that x is related to A by R. A partition P, represents all of the different equivalence classes of R.

# Cryptography and Modular Arithmetic

The following encryption method is called the Caesar cipher or shift cipher. Define each letter of the alphabet by the number listed below it in the given table.

|A|B|C|D|E|F|G|H|I|J|K|L|M|
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|1|2|3|4|5|6|7|8|9|10|11|12|13| 
|N|O|P|Q|R|S|T|U|V|W|X|Y|Z |
|14|15|16|17|18|19|20|21|22|23|24|25|26|

Definition: Plaintext is the information to be encrypted. Ciphertext is encrypted plaintext. 

1) Encrypt the plaintext: “Agents of Shield” using the formula C(x) = (P(x) + 8) (mod 26) Solution: first write the plaintext using numbers from the table above. 
		A G E N T S O F S H I E L D 
		1 7 5 14 20 19 15 6 19 8 9 5 12 4 

3) Then add 8 to each value. 
	A G E N T S O F S H I E L D 
	9 15 13 22 28 27 23 14 27 16 17 13 20 12 

4) For any values over 26, subtract 26 to get the modulus remainder. (if a value is negative or 0, add 26.) 
	A G E N T S O F S H I E L D 
	9 15 13 22 2 1 23 14 1 16 17 13 20 12 

5) Then rewrite the numbers as letter using the table. 
	9 15 13 22 2 1 23 14 1 16 17 13 20 12
	I O M V B A W N A P Q M T L 

7) Ciphertext: IOMVBAWNAPQMTL 

To decrypt the ciphertext, we would use the same process with P(x) = (C(x) ─ 8) (mod 26)