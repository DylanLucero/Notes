In this chapter, we will learn how to count the number of elements in more complicated sets.

Recall from Chapter 5 the definition of [[Section 5.3 - Equivalence Classes#^82b94b|partition]].

#### Theorem:
The addition rule states that if a set A can be written as a finite partition of subsets such that $A = P_1 \cup P_2 \;\cup\; ... \; \;\cup\; P_n$ with $P_n \;\cap\;P_j = \not 0$ for all $i,\;j$ then $|A|= |P_1|+|P_2|\;+\;...\; |P_n|$.

# The Addition Rule and Partitions
Determine the number of possibilities for each of the following scenarios.

a) You are choosing a song to download. Five of the songs are classic rock, 6 of the songs are hip hop, and 10 of the songs are jazz. How many different options do you have to download a song?

Solution: We can assume that none of the music genres are overlapping, meaning, a song cannot be both classic rock and hip hop. In math terms, the intersection of the genres is empty.

To formalize this mathematically, we can write

$R =$ the rock songs           $H =$ the hip hop songs           $J =$ the jazz songs

$$|R|=5 \;\;\;\;\;          |H|=6     \;\;\;\;\;               |J|=10$$

$$R∩H=R∩J=H∩J=∅$$

$$|R∪H∪J|=|R|+|H|+|J|=5+6+10 $$

This type of formalization is not necessary, but it is good to see how this specifically relates to the theorem. We can simply our solution as,

$5 + 6 + 10 = 21$

Answer: We have 21 different options for choosing a song to download.

  
b) At a restaurant, your meal comes with wither soup or salad. There are 5 types of soups and 3 types of salads. How many options do you have for a soup or salad when ordering your meal?

Solution: To formalize this mathematically, we can write

$P = the\;soup\;options \;\;\;\;\; D = the\;salad\;options$

 $$|P|=5        \;\;\;\;\; |D|=3$$

$$P∩D= ∅$$ 

$$|P∪D|=|P|+|D|=5+3=8$$

Or more simply, $5 + 3 = 8$ 
Answer: You have 8 options for ordering a soup or salad with your meal.

Notes:  
Observe that we are using the word “or” in these problems which corresponds to union.  
We will use the word “choice” as a verb for the action of choosing “options”. In everyday language, “choices” and “options” are nouns that are synonymous. For example, if you were at the restaurant, you might say, “what are my choices” or “what are my options”. This is fine, but it will reduce confusion if we agree to use choice only as a verb and not as a noun and options as a noun.

# The Inclusion/Exclusion Principle
We may encounter an “or” problem where the set is not given as a partition. In particular, the intersection of the different categories or attributes may not be empty. In these cases, we will use the Inclusion/Exclusion Principle which we briefly discussed in the Set Theory chapter.

The Inclusion/Exclusion Principle for two or three sets: Let A, B, and C be finite sets.  
Two Sets: $|A∪B|=|A|+|B|−|A∩B|$
Three Sets: $|A∪B∪C|=|A|+|B|+|C|−|A∩B|−|A∩C|−|B∩C|+|A∩B∩C|$

Justify the Inclusion/Exclusion Principle using Partitions of Venn Diagrams

a)  Two Sets

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1636616901101-0.png)

b)  Three Sets

![](https://moer.maricopa.edu/filestore/ufiles/2745/pastedimage1636616901101-1.png)

## Applying the Inclusion/Extrusion Principle
a) Dani recorded the hair color and eye color of 71 people. She then categorized them based on whether they had brown hair (or not) and blue eyes (or not). She found that  
  
42 people in total had brown hair  $H$
23 people in total had blue eyes.  $E$
8 people had both brown hair and blue eyes $H \cap E$

How many people had brown hair or blue eyes?

Since we are looking for either brown hair or blue eyes and not both, we can show this as: 
$|H\cup E|$ which equates to $H+E-(H \cap E)$

So, $$|H\cup E| = 42 (H) + 23(E) - 8(H\cap E) = 65 - 8 = 57$$

b) 156 students were surveyed on their current enrollment in Math, Biology, and Chemistry. The results are listed below.

  
59 students are enrolled in Math.  $A$
63 students are enrolled in Biology.  $B$
74 students are enrolled in Chemistry.  $C$
23 students are enrolled in Math and Bio.  $A \cap B$
21 students are enrolled in Bio and Chem.  $B \cap C$
22 students are enrolled in Math and Chem.  $A \cap C$
9 students are enrolled in all three courses. $A\cap B \cap C$

How many students were enrolled in at least one of the three courses?$$|A∪B∪C|=|A|+|B|+|C|−|A∩B|−|A∩C|−|B∩C|+|A∩B∩C|$$
This equates to:
$$59+63+74-23-21-22+9=139$$
