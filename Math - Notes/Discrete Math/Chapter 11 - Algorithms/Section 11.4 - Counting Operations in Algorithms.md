In this section, we are going to count the number of operations in some common algorithmic forms. We will use the two main theorems from counting from Chapter 8 listed below.

  
Theorem: The _**addition rule**_ states that if a set A can be written as a finite partition of subsets such that A=P1∪P2∪...∪Pn�=�1∪�2∪...∪�� with Pi∩Pj=��∩��=  ∅∅ for all i, j, then |A|=|P1|+|P2|+...+|Pn||�|=|�1|+|�2|+...+|��| 

  
Theorem (multiplication rule): If you have n choices to make and mj��  options for the jth choice, 1≤j≤n1≤�≤� , the total number of ways to make the n choices is

  
m1×m2× ... ×mn�1×�2× ... ×�� 

  
Definition: An _**algorithm**_ is a list of instructions for accomplishing a task.

  
We are going to use pseudocode in this section to describe algorithms. This way, we do not have to all be familiar with the same computer code. It will be described and defined as we go.

Assignment of a variable: To set the variable x to the value of y, we will write x ← y.

This changes the value of the variable x in storage to the new value of y. We can also use the same variable such as x ← x + 2 which means replace the value of x with the new value of x + 2. So if x = 3, after running x ← x + 2, the new value of x would be 5 and the 3 would be discarded and replaced with 5 in storage.

Conditional Statements: Sometimes we want to execute a process only under certain conditions. We use the form If (condition) then (statement). For example, if x > 0 then x ← x + 2.

Here is some code with outputs so we can read the results.

print “Initial value of x:” x  
if x > 0 then x ← x + 2  
print “New value of x:” x

For x = 3, since 3 > 0, the output would be:  
Initial value of x: 3  
New value of x: 5

For x = ‒2, since ‒2 < 0, the output would be:  
Initial value of x: ‒2  
New value of x: ‒2

Comments: We will use // proceeding a comment that is not part of the code.

# Sequences of Operations
Find the number of operations performed in the pseudocode below.

  
y ← x + x + x // line 1  
z ← y + y + y + y // line 2

Solution: In line 1, addition is performed twice. Then the result is added together 3 times in line 2. So the total number of additions is 2 + 3 = 5. This aligns with the addition principle of counting. Note: Be careful to count the number of operations and not the number of terms.

  
Answer: 5 operations

# For Loops
If an algorithm needs to repeat a process on multiple inputs, we can use a for-loop.

Definition:  Let I be a totally ordered set with n elements.  The **_for–loop_** below will execute statement n times, once for each .

for i∈I�∈�  do

      statement

**Problem 14:  Written Example –** for loops

Enumerate the algorithm below for n = 4.  Then count the number of operations in terms of n.

x ← 0                                  // line 1

for  i∈{1,2,...,n}�∈{1,2,...,�}  do     // line 2

       x ← x + i

Solution:  Let n = 4. 

x initializes at 0. 

- for i = 1, x is updated to 0 + 1 = 1
- for i = 2, x is updated to 1 + 2 = 3
- for i = 3, x is updated to 2 + 3 = 5
- for i = 4, x is updated to 3 + 4 = 7

The algorithm runs 4×1=44×1=4  operations.  For any natural number n, the algorithm runs n×1=n�×1=�  operations.

# Nested Loops
Definition: Let I and J be a totally ordered sets with n and m elements respectively. Then the nested–loop below will execute statement n x m times, once for each i ∈ I� ∈ �  and repeated for each j ∈ J� ∈ � .

for i ∈ Ido� ∈ ���   
       for  j∈J do �∈� ��   
          statement

  
**Problem 15: Written Example** – Nested Loops  
Enumerate the algorithm below for n = 2 and m = 3. Then count the number of operations in terms of n and m.  
Let A = { 1, 2, …,n} and B = {1, 2, …m}

for i ∈ A� ∈ �  do  
     for  j∈B �∈�  do   
          if i < j the print (i,j)

when n = 2 and m = 3  
for i ∈ {1, 2}� ∈ {1, 2}  do  
     for ![image](https://moer.maricopa.edu/cgi-bin/mimetex.cgi?%5Cdisplaystyle%5C%20%7Bj%7D%5Cin%7B%5Cleft%5Clbrace%7B1%7D%2C%5C%20%7B2%7D%2C%5C%20%7B3%7D%5Cright%5Crbrace%7D%60 "\ j\in{1,\ 2,\ 3}`")  do  
          if i<j�<�  the print (i,j)

1) i = 1 and  j = 1

1 = 1   (1,1) is not printed

  
2) i = 1 and j = 2  
1 < 2, (1,2) is printed

  
3) i = 1 and j = 3  
1 < 3, (1,3) is printed

  
4) i = 2 and j = 1  
2 > 1, (2,1) is not printed

  
5) i = 2 and  j = 2  
2 = 2, (2,2) is not printed

  
6) i = 2 and  j = 3  
2 < 3, (2,3) is printed

  
The algorithm runs 2×3=62×3=6  operations. For any natural numbers n and m, the algorithm runs n×m=nm�×�=��  operations.

# Nested Loops with Addition Principle

This algorithm lists the number of strings formed from the letters a through j of length 3 or less without repetitions.  Count the number of operations in each loop and determine the total number of operations.

``` C
Let D = {a, b, c, d, e, f, g, h, i, j}

for x∈D  do         //line 1

   print x         //line 2

for  x∈D�∈�  do //line 3

   for y∈D/{x}�∈�/{�}   do   //line 4

		 print xy   //line 5

for x∈D�∈� do    //line 6

            for y∈D/{x}�∈�/{�}  do   //line 7

                        for z∈D/{x,y}�∈�/{�,�}  do      //line 8

                                    print xyz         //line 9
```

Solution:  Lines 1 and 2 print the one letter strings.  There are 10.

Lines 3 through 5 print the two letter strings without repetition.  There are 10×9 .

Lines 6 through 9 print the three letter strings without repetition.  There are 10×9×8 .

Since these 3 types of string lengths are disjoint, we add them to find the total number of operations:  10 + 90 + 720 = 820

Answer:  There are 820 operations performed in this algorithm.

