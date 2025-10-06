We have two choices. We can try to generalize the factorial function to work with ﬂoating-point numbers, or we can make factorial check the type of its argument. The ﬁrst option is called the gamma function and it’s a little beyond the scope of this book. So we’ll go for the second.

We can use the built-in function isinstance to verify the type of the argument. While we’re at it, we can also make sure the argument is positive: def factorial (n):

if not isinstance(n, int):

’

print return None

Factorial is only defined for integers.

’

elif n < 0: ’

print return None

Factorial is not defined for negative integers.

’

elif n == 0: return 1

else:

return n * factorial(n-1)