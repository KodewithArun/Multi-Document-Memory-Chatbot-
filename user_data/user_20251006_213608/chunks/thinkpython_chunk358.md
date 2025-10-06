141

142

Chapter 14. Files

Chapter 15

Classes and objects

Code examples from this chapter are available from http://thinkpython.com/code/ Point1.py; solutions to the exercises are available from http://thinkpython.com/code/ Point1_soln.py.

15.1 User-deﬁned types

We have used many of Python’s built-in types; now we are going to deﬁne a new type. As an example, we will create a type called Point that represents a point in two-dimensional space.

In mathematical notation, points are often written in parentheses with a comma separating the coordinates. For example, (0,0) represents the origin, and (x,y) represents the point x units to the right and y units up from the origin.

There are several ways we might represent points in Python:

We could store the coordinates separately in two variables, x and y.

We could store the coordinates as elements in a list or tuple.

We could create a new type to represent points as objects.