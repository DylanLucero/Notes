# Definition
>A sequence is an ordered list of numbers with a domain of the natural numbers or positive integers.

^0a3f5d

### Notation
>We’ll usually use subscripts for a sequence instead of function notation:  a(n) = $a_n$ and $a_k$ is the $k^{th}$ **_term_** of the sequence.  The letter k is called the **_subscript or index_**.

^def
# Examples

Find the first 5 terms of the following sequences and then write the sequence in list form.

### 1) Let $a_k = \frac{k}{(k+1)}$ for $k >= 1$
#### Solution

Just plug k in and increment.

$a_1$ = $\frac{1}{(1 + 1)}$ = $\frac{1}{2}$
$a_2$ = $\frac{2}{(2 + 1)}$ = $\frac{2}{3}$
$a_3$ = ...

### 2) $b_i$ = $(-1)^{i + 1}$ for $i >= 0$

^5d49c4

#### Solution
$b_0$ = $(-1)^{0 + 1}$ = -1
$b_1$ = $(-1)^{1+1}$ = 1
$b_2$ = $(-1)^{2+1}$ = -1
$b_3$ = ...
>Note: We call sequences of this form **_alternators_** since they change signs every consecutive term.  They are often a factor in a sequence.

^f828f2
#### 3) $c_n$ = $(-1)^{n - 1}$$(\frac{1}{n})$ for $n >= 1$
#### Solution
$c_1$ = $(-1)^{1 - 1}$$(\frac{1}{1})$ = 1
$c_2$ = $(-1)^{2 - 1}$$(\frac{1}{2})$ = $-\frac{1}{2}$
$c_3$ = $(-1)^{3 - 1}$$(\frac{1}{3})$ = $-\frac{1}{3}$
$c_4$ = ...
>Note:  This sequence has an alternator, so we call it an alternating sequence.  Specifically, this sequence is the alternating harmonic sequence.  ( $a_n$ = $\frac {1}{n}$  is called the harmonic sequence.)

^harmonic
# Finding a formula for a sequence
## Example
#### a) $1, \frac{1}{4}, \frac{1}{9}, \frac{1}{16}, \frac{1}{25}, ...$
Notice the numerator is always 1, this means we can place a 1 in the numerator.
$$\frac{1}{?}$$
Looking at the denominators, we can see that it is $n^2$. This is because $1^2 = 1$, $2^2 = 4$, $3^2 = 9$, $...$

So the entire formula is:
$$a_n = \frac{1}{n^2}$$



#### b) $\frac{1}{2}, -\frac{2}{4}, \frac{3}{8}, -\frac{4}{16}, \frac{5}{32}, -\frac{6}{64}$
Notice the numerators are incrementing by 1. We can say our numerator is n. $$\frac{n}{?}$$
Also notice we have a alternator series as well since the sign is flip flopping. Recall our [[#^f828f2|note]] about alternating series. Using what we learned from the [[#^5d49c4|example]] we did on alternating series. This makes our formula look like: $$(-1)^{n + 1} (\frac{n}{?})$$
Now lets look at the denominator. Notice the pattern of 2, 4, 8, 16, 32, 64...
This pattern is easily recognizable as $2^n$.

Our final formula is:$$(-1)^{n + 1} (\frac{n}{2^n})$$