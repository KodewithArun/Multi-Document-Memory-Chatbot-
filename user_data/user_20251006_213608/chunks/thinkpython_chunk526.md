216

Appendix C. Lumpy

object

Pointxy

Rectanglecornerheightwidth

Figure C.7: Class diagram.

But if you are passing functions and classes as parameters, you might want them to appear. This example shows what that looks like; you can download it from http://thinkpython. com/code/lumpy_demo6.py.

import copy from swampy.Lumpy import Lumpy

lumpy = Lumpy() lumpy.make_reference()

class Point(object):

"""Represents a point in 2-D space."""

class Rectangle(object):

"""Represents a rectangle."""

def instantiate(constructor):

"""Instantiates a new object.""" obj = constructor() lumpy.object_diagram() return obj

point = instantiate(Point)

Figure C.6 shows the result. Since we invoke object_diagram inside a function, we get a stack diagram with a frame for the module-level variables and for the invocation of instantiate.

At the module level, Point and Rectangle refer to class objects (which have type type); instantiate refers to a function object.