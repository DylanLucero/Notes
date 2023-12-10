Conditional probabilities involve finding the probability of an event when you are given some additional knowledge or information about the observation or experiment. For example, suppose we have heart disease data for people over 50. We can use this data to calculate the probability of a random person over 50 having heart disease.

  
Now suppose the data are also partitioned by gender (male or female). We could also calculate probabilities of heart disease for a specific gender, perhaps the probability of heart disease of a person over 50 given that the person is a woman. The results could be different (and likely will in this case) if you use this new information. Similarly, the “given” information could be reversed. We could find the probability that a person over 50 is a woman given that they have heart disease. Note that although these are similar, the known information is different. In one case you know the person is a woman, and in the other, you know the person has heart disease. These probabilities are considering different subsets of people from the original population at the start and the probabilities are most likely different.

  
In the next example, we will compute some conditional probabilities using the method of reducing the sample space. The idea is, instead of looking at the original sample space of all equally likely outcomes, we will only consider the subset of the sample space that applies to our specific “given” information.

# Conditional Probability
Compute the following conditional probabilities by reducing the sample space.

a) A single die is rolled.

  
i. What is the probability the die is a 6 given that the roll is an even number?

Solution: First consider the original sample space of the experiment. Then reduce the sample space using the given information that the roll is an even number.  
![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid0_5.png)  
Using the reduced samples space, S = { 2, 4, 6 }, the total possible number of equally likely outcomes is 3. The event space, E = the die is a 6, is { 6 } which has one outcome. So the probability is 1 out of 3 or 1313 .  
Answer: 1313 

  
ii. What is the probability the die is an even number given that the roll is a 6?

Solution: First consider the original sample space of the experiment. Then reduce the sample space using the given information that the roll is a 6.  
![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid1_3.png)  
Using the reduced samples space, S = { 6 }, the total possible number of equally likely outcomes is 1. The event space, E = the die is even, is { 6 } which is also one outcome. Note that even though there are other even numbers in the original sample space, there are not any in the reduced sample space so we do not consider them in our computations. So the probability is 1 out of 1, 1111  or just 1. Note that this is a certain event. If we know the die is a 6, it is certainly also an even number.  
Answer: 1

  
_**Notice the probability of E1 given E2 is not necessarily equal to the probability of E2 given E1.**_

b) A card is drawn from a deck of 52 cards. What is the probability the card is a 5 given that the card is a number card? (Note: Aces are not considered number cards.)

  
Solution: First consider the original sample space of the experiment, the 52 cards, and then construct the reduced sample space with only number cards.  
![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid2_3.png)  
The number of elements in the reduced sample space is 36, and 4 of these cards are 5’s. So the probability is 4 out of 36, 436=19436=19 .

Answer:  1919 

  
c) Two cards are drawn from a deck of 52 cards.

i. What is the probability the second card is a diamond given that the first card is a diamond?

  
Solution: The sample space of all the possible outcomes for drawing two cards from a deck of cards is a bit complex. We can list all of the possible outcomes, but there are so many, it would likely make things more confusing. So let’s consider the two draws separately using the given information as shown in the image below.

![](https://moer.maricopa.edu/filestore/ufiles/2745/blobid3_3.png)  
Note for the second card, there are only 51 possible cards that can be drawn since we are given that the first card is a diamond. Specifically, there are still 13 clubs, 13 spades, 13 hearts, but only 12 diamonds. So there are 51 cards in the sample space for the second card. Since we are considering the event, E, that the second card is also a diamond, there are 12 diamonds in the sample space that are in this event space. So the probability is 12 out of 51 or  1251=4171251=417 

  
Answer: 417417 

  
ii. What is the probability the second card is a club given that the first card is a diamond?

  
Solution: Notice that this problem is similar to part i except that we want the probability that the second card is a club. It may seem like this probability wouldn’t change since the first card was a diamond and not a club. However, this sample space for the second card is the same as part i. The number of possible outcomes in the sample space has been reduced from 52 to 51 by the first card being chosen. There are 13 clubs in the reduced sample space. So the probability is 13 out of 51 or 13511351 .

  
Answer: 13511351

# Contingency Tables and Conditional Probability
  
A teacher categorized students by whether they regularly completed their homework (or not) and whether they passed the course (or not). The data are in the table below.

|                         | Completed Homework | Did not Complete Homework | Total |
| ----------------------- | ------------------ | ------------------------- | ----- |
| Passed the Course       | 52                 | 11                        | 63    |
| Did not Pass the Course | 6                  | 31                        | 37    |
| Total                   | 58                 | 42                        | 100   |

A student is randomly selected from this group of students. Use this information to find the probabilities requested. Enter all of your results as percents rounded to two decimal places.

a) What is the probability that a student completed the homework given that they passed the course?

b) What is the probability that a student passed the course given that they completed the homework?

c) What is the probability that a student completed the homework given that they did not pass the course?

d) What is the probability that a student did not pass the course given that they did not complete the homework?