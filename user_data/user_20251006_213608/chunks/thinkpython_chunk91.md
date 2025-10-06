’

3.14159

’

)

Finally, str converts its argument to a string: >>> str(32) ’

’

32

>>> str(3.14159) ’ ’

3.14159

3.3 Math functions

Python has a math module that provides most of the familiar mathematical functions. A module is a ﬁle that contains a collection of related functions.

Before we can use the module, we have to import it:

>>> import math

This statement creates a module object named math. If you print the module object, you get some information about it:

>>> print math ’ <module

’

math

(built-in)>

The module object contains the functions and variables deﬁned in the module. To access one of the functions, you have to specify the name of the module and the name of the function, separated by a dot (also known as a period). This format is called dot notation.

>>> ratio = signal_power / noise_power >>> decibels = 10 * math.log10(ratio)

>>> radians = 0.7 >>> height = math.sin(radians)