def absolute_value(x):

if x < 0:

return -x

else:

return x

52

Chapter 6. Fruitful functions

Since these return statements are in an alternative conditional, only one will be executed.

As soon as a return statement executes, the function terminates without executing any subsequent statements. Code that appears after a return statement, or any other place the ﬂow of execution can never reach, is called dead code.

In a fruitful function, it is a good idea to ensure that every possible path through the pro- gram hits a return statement. For example:

def absolute_value(x):

if x < 0:

return -x

if x > 0:

return x

This function is incorrect because if x happens to be 0, neither condition is true, and the function ends without hitting a return statement. If the ﬂow of execution gets to the end of a function, the return value is None, which is not the absolute value of 0.

>>> print absolute_value(0) None