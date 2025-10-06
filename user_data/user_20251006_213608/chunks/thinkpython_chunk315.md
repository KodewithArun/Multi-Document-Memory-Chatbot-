The function random returns a random ﬂoat between 0.0 and 1.0 (including 0.0 but not 1.0). Each time you call random, you get the next number in a long series. To see a sample, run this loop:

import random

for i in range(10):

x = random.random() print x

The function randint takes parameters low and high and returns an integer between low and high (including both).

>>> random.randint(5, 10) 5 >>> random.randint(5, 10) 9

To choose an element from a sequence at random, you can use choice:

>>> t = [1, 2, 3] >>> random.choice(t) 2 >>> random.choice(t) 3

The random module also provides functions to generate random values from continuous distributions including Gaussian, exponential, gamma, and a few more. Exercise 13.5. Write a function named choose_from_hist that takes a histogram as deﬁned in Section 11.1 and returns a random value from the histogram, chosen with probability in proportion to frequency. For example, for this histogram: ’

’

’

’

’

’

a

,

b

,