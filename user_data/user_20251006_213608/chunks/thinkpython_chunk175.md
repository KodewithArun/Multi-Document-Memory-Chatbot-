’

elif n == 0: return 1

else:

return n * factorial(n-1)

The ﬁrst base case handles nonintegers; the second catches negative integers. In both cases, the program prints an error message and returns None to indicate that something went wrong: >>> factorial( Factorial is only defined for integers. None >>> factorial(-2) Factorial is not defined for negative integers. None

’

’

fred

)

6.9. Debugging

If we get past both checks, then we know that n is positive or zero, so we can prove that the recursion terminates.

This program demonstrates a pattern sometimes called a guardian. The ﬁrst two condi- tionals act as guardians, protecting the code that follows from values that might cause an error. The guardians make it possible to prove the correctness of the code.

In Section 11.3 we will see a more ﬂexible alternative to printing an error message: raising an exception.

6.9 Debugging