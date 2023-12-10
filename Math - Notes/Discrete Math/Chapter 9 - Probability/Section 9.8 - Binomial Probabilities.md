Definition: Let the result of a random experiment have two possible outcomes, X = 0 and X = 1, where X = 1 means success and X = 0 means failure. Let P(1) = pandP(0) = 1 −p�(1) = �and�(0) = 1 -� . This type of trial is called a _**Bernoulli experiment**_.

  
Examples:

a) Flipping a coin where a head counts as success and tails counts as a failure.

b) Testing someone for a disease where having the disease counts as success and not having the disease counts as failure.

c) Rolling a die where an even number counts as success and an odd number counts as a failure.

Note: “Success” and “failure” don’t necessarily mean something good or bad. It is just a way to distinguish between the two possible outcomes and indicate which we are trying to measure.

Definition: Now suppose that the Bernoulli experiment is repeated for n independent trials. A binomial random variable, X, represents the number of successes out of the n independent trials. The probability X = k where 0≤k≤n0≤�≤�  is computed using the Binomial theorem and equals

  
  
 P(X=k)=(nk)pk(1−p)n−k�(�=�)=(��)��(1-�)�-�
# Binomial Probability of Flipping a Coin
Suppose a fair coin is flipped 3 times. Find the probability of getting 0 heads, 1 head, 2 heads, and 3 heads.

Solution: We will use the binomial theorem to compute these, but first let’s enumerate the possibilities to see how the formula connects to the results. There are 8 equally likely outcomes.

Ways to get 0 heads: TTT                                P(X=0)=18�(�=0)=18   
Ways to het 1 head: HTT, THT, TTH               P� (X=1)=38(�=1)=38   
Ways to get 2 heads: THH, HTH, HHT          P(X=2)=38�(�=2)=38   
Ways to get 3 heads: HHH                              P(X=3)=18�(�=3)=18 

 P(X=0)=(30)(12)0(1−12)3−0= 1×(12)3=18�(�=0)=(30)(12)0(1-12)3-0= 1×(12)3=18 

P(X=1)=(31)(12)1(1−12)3−1= 3×(12)3=38�(�=1)=(31)(12)1(1-12)3-1= 3×(12)3=38   
P(X=2)=(32)(12)2(1−12)3−2= 3×(12)3=38�(�=2)=(32)(12)2(1-12)3-2= 3×(12)3=38   
P(X=3)=(33)(12)3(1−12)3−3= 1×(12)3=18�(�=3)=(33)(12)3(1-12)3-3= 1×(12)3=18

# Binomial Probability
a) A die is rolled 8 times. What is the probability it lands on 3 exactly 5 times?

  
b) A fair coin is flipped 5 times. What is the probability it lands on heads 3 or more times?

  
c) A company knows that the probability that one of its products is defective is 0.01. The probability of any product being defective is independent of the others. The product is sold in packages of 10. If the company offers a money back guarantee if any of the products in the package are defective, what proportion of the packages will the company need to reimburse?

Solutions:  
a) The probability of rolling a 3 on any trial is 1616 . The probability of not rolling a 3 is 5656 . The number of trials is n = 8 and the number of successes is k = 5.

 P(X=5)=(85)(16)5(56)3�(�=5)=(85)(16)5(56)3 

 P(X=5)=56×125×(16)8�(�=5)=56×125×(16)8 

 P(X=5)=56×125×11,679,616≈0.00417�(�=5)=56×125×11,679,616≈0.00417 

Answer: 0.00417

  
b) The probability of flipping a head on any trial is 1212 . The probability of not flipping a head is 1212 . The number of trials is n = 5 and the number of successes is k = 3, k = 4, or k = 5. Since these k values are mutually exclusive, we can find all three and add the results.

  
P(X=3)=(53)(12)3(12)2�(�=3)=(53)(12)3(12)2   
 P(X=4)=(54)(12)4(12)1�(�=4)=(54)(12)4(12)1   
P(X=5)=(55)(12)5(12)0�(�=5)=(55)(12)5(12)0 

Now add the results. Notice that all of the probabilities have a factor of (12)5(12)5 . Factoring this out of the sum yields:

  
 ((53)+(54)+(55))(12)5=(10+5+1)(12)5=16(12)5=24×125=12((53)+(54)+(55))(12)5=(10+5+1)(12)5=16(12)5=24×125=12 

Answer: 1212 

c) The probability of a defective product on any trial is 0.01. The probability a product is not defective is 0.99. The number of trials is n = 10 since there are 10 products per package. If we define success as one or more of the products being defective, then we would need to find and add the probabilities for X equal to 1, 2, ..,10. Instead, we will find the probability that 0 of the products are defective and subtract the result from 1 using the complement rule. So let k = 0.

P(X=0)=(100)(0.01)0(0.99)10=1×1×(0.99)10≈0.904�(�=0)=(100)(0.01)0(0.99)10=1×1×(0.99)10≈0.904 

This means, approximately 90.4% of the time, none of the products in a package of 10 will be defective. So 100% - 90.4% = 9.6% of the time, at least one of the products in the package of 10 will be defective.

  
Answer: The company will need to reimburse the cost for 9.6% of the packages it sells.