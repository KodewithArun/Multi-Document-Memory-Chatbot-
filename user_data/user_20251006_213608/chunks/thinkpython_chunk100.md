What’s the moral of this sordid tale? When you read a program, you don’t always want to read from top to bottom. Sometimes it makes more sense if you follow the ﬂow of execution.

3.8 Parameters and arguments

Some of the built-in functions we have seen require arguments. For example, when you call math.sin you pass a number as an argument. Some functions take more than one argument: math.pow takes two, the base and the exponent.

Inside the function, the arguments are assigned to variables called parameters. Here is an example of a user-deﬁned function that takes an argument:

def print_twice(bruce):

print bruce print bruce

This function assigns the argument to a parameter named bruce. When the function is called, it prints the value of the parameter (whatever it is) twice.

This function works with any value that can be printed.

23

24

Chapter 3. Functions

’

’

>>> print_twice( Spam Spam >>> print_twice(17) 17 17 >>> print_twice(math.pi) 3.14159265359 3.14159265359

Spam

)