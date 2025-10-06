e = math.exp(1.0) height = radius * math.sin(radians)

All of the functions we have written so far are void; they print something or move turtles around, but their return value is None.

In this chapter, we are (ﬁnally) going to write fruitful functions. The ﬁrst example is area, which returns the area of a circle with the given radius:

def area(radius):

temp = math.pi * radius**2 return temp

We have seen the return statement before, but in a fruitful function the return statement includes an expression. This statement means: “Return immediately from this function and use the following expression as a return value.” The expression can be arbitrarily complicated, so we could have written this function more concisely:

def area(radius):

return math.pi * radius**2

On the other hand, temporary variables like temp often make debugging easier.

Sometimes it is useful to have multiple return statements, one in each branch of a condi- tional:

def absolute_value(x):

if x < 0: