’

__main__.Point

>

The class object is like a factory for creating objects. To create a Point, you call Point as if it were a function. >>> blank = Point() >>> print blank <__main__.Point instance at 0xb7e9d3ac> The return value is a reference to a Point object, which we assign to blank. Creating a new object is called instantiation, and the object is an instance of the class.

When you print an instance, Python tells you what class it belongs to and where it is stored in memory (the preﬁx 0x means that the following number is in hexadecimal).

15.2 Attributes

You can assign values to an instance using dot notation: >>> blank.x = 3.0 >>> blank.y = 4.0 This syntax is similar to the syntax for selecting a variable from a module, such as math.pi or string.whitespace. In this case, though, we are assigning values to named elements of an object. These elements are called attributes.