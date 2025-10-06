We could create a new type to represent points as objects.

Creating a new type is (a little) more complicated than the other options, but it has advan- tages that will be apparent soon.

A user-deﬁned type is also called a class. A class deﬁnition looks like this:

class Point(object):

"""Represents a point in 2-D space."""

This header indicates that the new class is a Point, which is a kind of object, which is a built-in type.

The body is a docstring that explains what the class is for. You can deﬁne variables and functions inside a class deﬁnition, but we will get back to that later.

Deﬁning a class named Point creates a class object.

144

Chapter 15. Classes and objects

xy3.04.0blankPoint

Figure 15.1: Object diagram.

>>> print Point ’ <class Because Point is deﬁned at the top level, its “full name” is __main__.Point.

’

__main__.Point

>