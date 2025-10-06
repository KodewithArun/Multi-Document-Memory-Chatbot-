6. Turn left 60 degrees.

7. Draw a Koch curve with length x/3.

The exception is if x is less than 3: in that case, you can just draw a straight line with length x.

1. Write a function called koch that takes a turtle and a length as parameters, and that uses the turtle to draw a Koch curve with the given length.

2. Write a function called snowflake that draws three Koch curves to make the outline of a snowﬂake.

Solution: http://thinkpython.com/code/koch.py.

3. The Koch curve can be generalized in several ways. See http://en.wikipedia.org/ wiki/Koch_snowflake for examples and implement your favorite.

Chapter 6

Fruitful functions

6.1 Return values

Some of the built-in functions we have used, such as the math functions, produce results. Calling the function generates a value, which we usually assign to a variable or use as part of an expression.

e = math.exp(1.0) height = radius * math.sin(radians)