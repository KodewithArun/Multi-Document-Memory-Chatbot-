There are at least two possibilities:

You could specify one corner of the rectangle (or the center), the width, and the height.

You could specify two opposing corners.

At this point it is hard to say whether either is better than the other, so we’ll implement the ﬁrst one, just as an example.

Here is the class deﬁnition:

class Rectangle(object):

"""Represents a rectangle.

attributes: width, height, corner. """

The docstring lists the attributes: width and height are numbers; corner is a Point object that speciﬁes the lower-left corner.

To represent a rectangle, you have to instantiate a Rectangle object and assign values to the attributes:

box = Rectangle() box.width = 100.0 box.height = 200.0

145

146

Chapter 15. Classes and objects

y0.0x0.0width100.0corner200.0PointRectangleboxheight

Figure 15.2: Object diagram.

box.corner = Point() box.corner.x = 0.0 box.corner.y = 0.0