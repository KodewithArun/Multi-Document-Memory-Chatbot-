(%g, %g)

% (blank.x, blank.y)

You can pass an instance as an argument in the usual way. For example:

def print_point(p): (%g, %g)

’

print

’

% (p.x, p.y)

print_point takes a point as an argument and displays it in mathematical notation. To invoke it, you can pass blank as an argument:

>>> print_point(blank) (3.0, 4.0)

Inside the function, p is an alias for blank, so if the function modiﬁes p, blank changes. Exercise 15.1. Write a function called distance_between_points that takes two Points as ar- guments and returns the distance between them.

15.3 Rectangles

Sometimes it is obvious what the attributes of an object should be, but other times you have to make decisions. For example, imagine you are designing a class to represent rectangles. What attributes would you use to specify the location and size of a rectangle? You can ig- nore angle; to keep things simple, assume that the rectangle is either vertical or horizontal.

There are at least two possibilities: