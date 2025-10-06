Inside the function, rect is an alias for box, so if the function modiﬁes rect, box changes. Exercise 15.2. Write a function named move_rectangle that takes a Rectangle and two numbers named dx and dy. It should change the location of the rectangle by adding dx to the x coordinate of corner and adding dy to the y coordinate of corner.

15.6 Copying

Aliasing can make a program difﬁcult to read because changes in one place might have unexpected effects in another place. It is hard to keep track of all the variables that might refer to a given object.

Copying an object is often an alternative to aliasing. The copy module contains a function called copy that can duplicate any object:

>>> p1 = Point() >>> p1.x = 3.0 >>> p1.y = 4.0

>>> import copy >>> p2 = copy.copy(p1)

p1 and p2 contain the same data, but they are not the same Point.

>>> print_point(p1) (3.0, 4.0) >>> print_point(p2) (3.0, 4.0) >>> p1 is p2 False >>> p1 == p2 False