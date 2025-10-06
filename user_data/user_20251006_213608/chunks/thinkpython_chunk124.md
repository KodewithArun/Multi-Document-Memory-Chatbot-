These are called keyword arguments because they include the parameter names as “key- words” (not to be confused with Python keywords like while and def).

This syntax makes the program more readable. It is also a reminder about how arguments and parameters work: when you call a function, the arguments are assigned to the param- eters.

4.6

Interface design

The next step is to write circle, which takes a radius, r, as a parameter. Here is a simple solution that uses polygon to draw a 50-sided polygon: def circle(t, r):

circumference = 2 * math.pi * r n = 50 length = circumference / n polygon(t, n, length)

The ﬁrst line computes the circumference of a circle with radius r using the formula 2πr. Since we use math.pi, we have to import math. By convention, import statements are usually at the beginning of the script.