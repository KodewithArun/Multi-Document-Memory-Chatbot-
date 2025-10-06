>>> type(32) ’ > <type

’

int

The name of the function is type. The expression in parentheses is called the argument of the function. The result, for this function, is the type of the argument.

It is common to say that a function “takes” an argument and “returns” a result. The result is called the return value.

3.2 Type conversion functions

Python provides built-in functions that convert values from one type to another. The int function takes any value and converts it to an integer, if it can, or complains otherwise:

’

’

32

>>> int( 32 >>> int( ValueError: invalid literal for int(): Hello

)

’

’

Hello

)

int can convert ﬂoating-point values to integers, but it doesn’t round off; it chops off the fraction part:

>>> int(3.99999) 3 >>> int(-2.3) -2

float converts integers and strings to ﬂoating-point numbers:

20

Chapter 3. Functions

>>> float(32) 32.0 >>> float( 3.14159

’

3.14159

’

)

Finally, str converts its argument to a string: >>> str(32) ’

’

32