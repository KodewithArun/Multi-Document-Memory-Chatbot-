vorpal: An adjective used to describe something that is vorpal.

If you saw that deﬁnition in the dictionary, you might be annoyed. On the other hand, if you looked up the deﬁnition of the factorial function, denoted with the symbol !, you might get something like this:

0! = 1 n! = n(n − 1)!

55

56

Chapter 6. Fruitful functions

This deﬁnition says that the factorial of 0 is 1, and the factorial of any other value, n, is n multiplied by the factorial of n − 1.

So 3! is 3 times 2!, which is 2 times 1!, which is 1 times 0!. Putting it all together, 3! equals 3 times 2 times 1 times 1, which is 6.

If you can write a recursive deﬁnition of something, you can usually write a Python pro- gram to evaluate it. The ﬁrst step is to decide what the parameters should be. In this case it should be clear that factorial takes an integer:

def factorial(n):

If the argument happens to be 0, all we have to do is return 1:

def factorial(n): if n == 0:

return 1