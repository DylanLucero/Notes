In this section, we will investigate independent events. Two events E1 and E2 are said to be _**independent**_ if the probability of E1 does not affect the probability of E2 or vice versa. Two events that are not independent events are called _**dependent events**_.

  
For example, if you flip a coin and roll a die, the outcome of the coin and the outcome of the die have no effect on one another, so the outcomes of the coin and the die are independent events. We can justify this mathematically using conditional probabilities. We can choose particular events (outcomes) of the die and coin and show that the probability of E1 given E2, is the same as the probability of E1 verifying that E2 has no effect on E1.

  
Fact: If the probability of E1 equals the probability of E1 given E2, then E1 and E2 are independent. If the probability of E1 does not equal the probability of E1 given E2, then E1 and E2 are dependent.

# Independent Events and Conditional Probability
**Part 1:**

  
A fair coin is flipped and a die is rolled. What is the probability the coin will land on heads? What is the probability the coin will land on heads given that the die lands on 3? Are the events of the coin landing on heads and the die landing on 3 independent?

  
**Solution**: First construct the sample space for the experiment of flipping a coin and rolling a die.

|Die<br><br>Coin|1|2|3|4|5|6|
|---|---|---|---|---|---|---|
|Heads (H)|H, 1|H, 2|H, 3|H, 4|H, 5|H, 6|
|Tails (T)|T, 1|T, 2|T, 3|T, 4|T, 5|T, 6|

a) What is the probability the coin will land on heads?

  
**Solution**: Observe the sample space has 12 equally likely outcomes. The event space for the coin landing on heads is boxed in blue below and contains 6 of the equally likely outcomes. So the probability of the coin landing on heads is 6 out of 12 or 612=12612=12   
![H1 H2 H3 H4 H5 H6 T1 T2 T3 T4 T5 T6](https://moer.maricopa.edu/filestore/ufiles/2745/mceclip4-1602823668540.png)  
**Answer:** 1212 

  
b) What is the probability the coin will land on heads given that the die lands on 3?

  
**Solution**: The outcomes where the die lands on 3 gives the reduced sample space, and are boxed in green from the original sample space in the diagram below.

![H1 H2 H3 H4 H5 H6 T1 T2 T3 T4 T5 T6](https://moer.maricopa.edu/filestore/ufiles/2745/mceclip5-1602823838506.png)  
  
So the reduced sample space is { H3, T3 } and contains two outcomes. One of these outcomes, namely, H3 has an outcome with heads. So the probability of heads given the die lands on 3 is 1 out of 2 or 1212 

**Answer**: 1212 

  
c) Are the events of the coin landing on heads and the die landing on 3 independent?

  
**Solution**: Since the probability the coin lands on heads and the probability the coin lands on heads given the die is a 3 are equal (both are 1212  ), the two events are independent.

  
**Answer**: Yes the two events are independent.

**Part 2:**

One card is drawn from a deck of 52 cards and the card is an Ace.

a) What is the probability that if you draw a second card the card is a 3 given that the Ace is returned to the deck?

  
**Solution**: Since you are given that the Ace is returned to the deck, there are 52 cards. Four out of the 52 cards are 3’s so the probability of drawing a 3 is 452=113452=113 

**Answer**: 113113 

b) What is the probability that if you draw a second card the card is a 3 given that the Ace is not returned to the deck?

**Solution**: Since the Ace is not returned to the deck, there are only 51 cards. Four out of the 51 cards are 3’s so the probability of drawing a 3 is 451451 

**Answer**: 4/51

c) Is drawing a second card that is a 3 independent of the first draw of the Ace when the Ace is returned to the deck?

**Solution**: The probability of drawing a club from the deck if there wasn’t a first card at all is 113113 . The probability of drawing a second card that is a club when an Ace is drawn, but returned to the deck is also 113113 . Since these probabilities are the same, the second card is independent of the first when the card is returned to the deck.

**Answer**: Independent

  
d) Is drawing a second card that is a 3 independent of the first draw of the Ace when the Ace is not returned to the deck?

**Solution**:  The probability of drawing a club from the deck if there wasn’t a first card at all is 113113  . The probability of drawing a second card that is a club when an Ace is drawn, and not returned to the deck is 451451 . Since these probabilities are the different, the second card is dependent on the first card when the card is not returned to the deck.

**Answer**: Dependent

  
**Notes**: In the first example, part a, the card was returned to the deck. This is called drawing the second card _**with replacement**_. In the second example, part b, the card was not returned to the deck. This is called drawing the second card _**without replacement**_. This idea will occur frequently in our discussion of probability since we often draw multiple cards from a deck without replacement.

  
Also observe that when we draw cards without replacement, a single card outcome of the 52 cards cannot be repeated. For example, you could not draw the Ace of Spades twice if it is not returned to the deck. We will also use the language without repetition corresponding to without replacement or repetition allowed corresponding to with replacement.

**Summary:**

1) Without repetition or without replacement events will be dependent.  
2) With repetition or with replacement events will be independent.
Recall that the intersection of two sets or events, E1∩E2�1∩�2 , means that E1�1  and E2�2  both occur. We have already computed some probabilities of two events occurring by examining the sample space. In this section we will develop formulas for finding these probabilities directly from the probabilities of the individual events, first for independent events and then dependent events.

# Independent Events and the Probability of their Intersection

The sample space for rolling a single die and flipping a coin is below. Let’s find the probability that the coin flip is heads, and the die roll is 5 using the sample space.

We can find the intersection of the events by determining the outcomes for each event, and then determining the intersection of the two events. The event that the coin flip is heads is highlighted in blue in the diagram below and to the right. This event space contains 6 outcomes out of 12, so the probability the coin toss is heads is 612=12612=12  . The event that the die is a 5 is highlighted in yellow in the diagram below the coin flip diagram. This event space contains 2 outcomes out of 12, so the probability the die is a 5 is 212=16212=16  . The intersection of the events, that the coin toss is a head and the die is a 5, contains one out of 12 outcomes, namely, H5. So the probability that both occur is 1 out of 12 or 112112 .

![H1 H2 H3 H4 H5 H6 T1 T2 T3 T4 T5 T6  First diagram H1 H2 H3 H4 H5 H6  highlighted.  Second diagram  H5 and T5 highlighted.](https://moer.maricopa.edu/filestore/ufiles/2745/mceclip6-1602825503084.png)

Recall from Problem 4, that the coin toss and die roll are independent events. Now that we know this concept, we can find the probability of the intersection in a different way.

  
The probability that the coin toss is heads and the die is a 5 equals:

probability the coin toss is heads × probability the die is a 5 is 12×16=11212×16=112 

Notice this corresponds to our previous result. Now we will summarize this fact in general.

# Product Rule for the Intersection of Independent Events

If two events E1�1  and E2�2  are independent, then  
The probability of E1andE2�1and�2  = the probability of E1�1  × the probability of E2�2

Determine the following probabilities using the product rule for the intersection of independent events.

a) Two coins are flipped. Find the probability that both coins land on heads.

b) Two cards are drawn from a deck of 52 cards. The first card is replaced before drawing the second card. Find the probability that the first card is a heart and the second card is a Jack.

c) A single digit between 0 and 9 is randomly chosen, and a single letter from A to Z is randomly chosen. Find the probability that the number is 7 and the letter is a vowel.

# Dependent Events and the Probability of Their Intersection
Two develop the intersection formula for two dependent events, let’s begin with a card problem. For simplicities sake, we will consider drawing 2 cards from a deck that only contains the 13 diamonds of a standard deck of cards. The 13 cards are shown below.

  
![13 diamond cards](https://moer.maricopa.edu/filestore/ufiles/2745/mceclip7-1602825956764.png)  
**Deck of 13 cards for Experiment**

  
The sample space for drawing two cards without replacement is shown in the table below. Observe that the diagonal from the top left to the bottom right is filled with X's and shaded gray. This is because we are drawing the two cards without replacement so it is impossible to draw the same card both 1st and 2nd. There are 156 equally likely possible outcomes for this experiment. This table is large and tedious to create, but once we have established our rule for the intersection of independent events, we will not need to do this again.

|1st card<br><br>2nd card|K|Q|J|10|9|8|7|6|5|4|3|2|A|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|K|**X**|Q,K|J,K|10,K|9,K|8,K|7,K|6,K|5,K|4,K|3,K|2,K|A,K|
|Q|K,Q|**X**|J,Q|10,Q|9,Q|8,Q|7,Q|6,Q|5,Q|4,Q|3,Q|2,Q|A,Q|
|J|K, J|Q, J|**X**|10, J|9, J|8, J|7, J|6, J|5, J|4, J|3, J|2, J|A, J|
|10|K,10|Q,10|J,10|**X**|9,10|8,10|7,10|6,10|5,10|4,10|3,10|2,10|A,10|
|9|K,9|Q,9|J,9|10,9|**X**|8,9|7,9|6,9|5,9|4,9|3,9|2,9|A,9|
|8|K,8|Q,8|J,8|10,8|9,8|**X**|7,8|6,8|5,8|4,8|3,8|2,8|A,8|
|7|K,7|Q,7|J,7|10,7|9,7|8,7|**X**|6,7|5,7|4,7|3,7|2,7|A,7|
|6|K,6|Q,6|J,6|10,6|9,6|8,6|7,6|**X**|5,6|4,6|3,6|2,6|A,6|
|5|K,5|Q,5|J,5|10,5|9,5|8,5|7,5|6,5|**X**|4,5|3,5|2,5|A,5|
|4|K,4|Q,4|J,4|10,4|9,4|8,4|7,4|6,4|5,4|**X**|3,4|2,4|A,4|
|3|K,3|Q,3|J,3|10,3|9,3|8,3|7,3|6,3|5,3|4,3|**X**|2,3|A,3|
|2|K,2|Q,2|J,2|10,2|9,2|8,2|7,2|6,2|5,2|4,2|3,2|**X**|A,2|
|A|K,A|Q,A|J,A|10,A|9,A|8,A|7,A|6,A|5,A|4,A|3,A|2,A|**X**|

**Sample Space for Drawing 2 of 13 cards Without Replacement**

Now let’s find a probability for this experiment in the next Worked Example.

Two cards are drawn from a deck of 13 diamond cards without replacement. Find the probability that the first card is a face card and the second card is a number card. (Note: Aces are not considered face or number cards).

**Solution 1**: The sample space below shows that the first 3 columns and 9 rows in the middle have outcomes where the first card is a face card and the second card is a number card. Observe that there are 27 out of 156 possible outcomes meet these requirements.

  
**Answer**: So the probability is 27156=95227156=952 

![Sample Space for Drawing 2 of 13 diamond cards Without Replacement  1st card face card and 2nd card number card highlighted](https://moer.maricopa.edu/filestore/ufiles/2745/mceclip8-1602826291946.png)

**Solution 2**: Now let’s consider finding the probabilities for the two events separately.

First we will find the probability the first card is a face card. Observe that there are 36 possible outcomes in the first three columns that have a first card that is a face card. So the probability the first card is a face card is 36156=31336156=313 .

Now we will find the probability that the second card is a number card given that the first card is a face card.

  
The table below shows the reduced sample space for the second card given that the first card is a face card. Observe that there are 36 possible outcomes, and 27 of these outcomes meet the requirement that the second card is a number card. So the probability that the second card is a number card given that the first card is a face card is 2736=342736=34 .

![Sample Space for Drawing 2 of 13 diamond cards Without Replacement  1st card face card and 2nd card number card highlighted](https://moer.maricopa.edu/filestore/ufiles/2745/mceclip9-1602826475857.png)  
Now let’s observe the product of the two probabilities before we simplified the fractions.

Probability 1st card is a face card: 3615636156 

Probability 2nd card is a number card given the 1st is a face card: 27362736 

Product:

![image](https://moer.maricopa.edu/filestore/ufiles/2745/mceclip10-1602826648874.png)

Observe that the numerator of the first probability equals the denominator of the second probability. This occurs because in the second probability, we reduce the sample space (denominator) to the outcomes from the first probability which is the first probability’s numerator.

  
Since this gives an identical factor in the numerator and denominator, these equal factors of 36 cancel to 1 resulting in the fraction 2715627156  which reduces to 913913 .

  
This fraction should look familiar. This was our unsimplified and simplified fractions from Solution 1 for this problem. This is not a coincidence. This result generalizes to all dependent probabilities as follows.

  
**Product Rule for the Intersection of Dependent Events:**

If two events E1�1  and E2�2  are dependent, then  
The probability of E1andE2�1and�2  = the probability of E1�1  × the probability of E2�2  given E1�1 

  
(**Note**: Since for independent events, the probability of E2�2  given E1�1  equals the probability of E2�2 , you can generally apply this formula to the intersection of any two events.)

Determine the following probabilities using the product rule for the intersection of dependent events.

a) Two names are drawn from a hat of 15 names without replacement to determine who will be responsible for driving to a sporting event. If there are 8 women and 7 men, what is the probability that the first person chosen is a man and the second person chosen is a woman?

b) Two cards are drawn from a deck of 52 cards without replacing the first card before choosing the second card. Find the probability that the first card is a club and the second card is a red Jack.

c) Two letters are chosen from A to Z for a password. The letters must be different from one another. Find the probability that the first letter is a vowel and the second letter is a Z.