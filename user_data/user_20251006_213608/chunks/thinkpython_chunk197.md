’

’

1 + 2 * 3

>>> eval( 7 >>> import math >>> eval( 2.2360679774997898 ’ >>> eval( <type

)

’

math.sqrt(5)

type(math.pi)

’

’

float

>

’

)

’

)

Write a function called eval_loop that iteratively prompts the user, takes the resulting input and evaluates it using eval, and prints the result.

’

’

It should continue until the user enters evaluated. Exercise 7.5. The mathematician Srinivasa Ramanujan found an inﬁnite series that can be used to generate a numerical approximation of 1/π:

done

, and then return the value of the last expression it

1 π

=

√

2 2 9801

∞ ∑ k=0

(4k)!(1103 + 26390k) (k!)43964k

69

70

Chapter 7. Iteration

Write a function called estimate_pi that uses this formula to compute and return an estimate of π. It should use a while loop to compute terms of the summation until the last term is smaller than 1e-15 (which is Python notation for 10−15). You can check the result by comparing it to math.pi.

Solution: http://thinkpython.com/code/pi.py.