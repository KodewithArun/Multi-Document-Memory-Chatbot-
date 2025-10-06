4.5 Generalization

The next step is to add a length parameter to square. Here is a solution:

def square(t, length): for i in range(4):

fd(t, length) lt(t)

square(bob, 100)

Adding a parameter to a function is called generalization because it makes the function more general: in the previous version, the square is always the same size; in this version it can be any size.

4.6. Interface design

The next step is also a generalization. Instead of drawing squares, polygon draws regular polygons with any number of sides. Here is a solution :rule

def polygon(t, n, length): angle = 360.0 / n for i in range(n):

fd(t, length) lt(t, angle)

polygon(bob, 7, 70)

This draws a 7-sided polygon with side length 70. If you have more than a few numeric arguments, it is easy to forget what they are, or what order they should be in. It is legal, and sometimes helpful, to include the names of the parameters in the argument list: polygon(bob, n=7, length=70)