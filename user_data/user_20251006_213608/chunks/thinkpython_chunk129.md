2. Once you get the program working, encapsulate it in a function and give it a name.

3. Generalize the function by adding appropriate parameters.

4. Repeat steps 1–3 until you have a set of working functions. Copy and paste working code to avoid retyping (and re-debugging).

5. Look for opportunities to improve the program by refactoring. For example, if you have similar code in several places, consider factoring it into an appropriately general function.

This process has some drawbacks—we will see alternatives later—but it can be useful if you don’t know ahead of time how to divide the program into functions. This approach lets you design as you go along.

4.9 docstring

A docstring is a string at the beginning of a function that explains the interface (“doc” is short for “documentation”). Here is an example:

def polyline(t, n, length, angle):

"""Draws n line segments with the given length and angle (in degrees) between them. """ for i in range(n):

t is a turtle.