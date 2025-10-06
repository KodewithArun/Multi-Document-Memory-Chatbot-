3.11 Fruitful functions and void functions

Some of the functions we are using, such as the math functions, yield results; for lack of a better name, I call them fruitful functions. Other functions, like print_twice, perform an action but don’t return a value. They are called void functions.

When you call a fruitful function, you almost always want to do something with the result; for example, you might assign it to a variable or use it as part of an expression:

x = math.cos(radians) golden = (math.sqrt(5) + 1) / 2

When you call a function in interactive mode, Python displays the result:

>>> math.sqrt(5) 2.2360679774997898

But in a script, if you call a fruitful function all by itself, the return value is lost forever!

math.sqrt(5)

This script computes the square root of 5, but since it doesn’t store or display the result, it is not very useful.