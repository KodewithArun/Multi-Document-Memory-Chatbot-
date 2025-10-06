Figure 15.2: Object diagram.

box.corner = Point() box.corner.x = 0.0 box.corner.y = 0.0

The expression box.corner.x means, “Go to the object box refers to and select the attribute named corner; then go to that object and select the attribute named x.”

Figure 15.2 shows the state of this object. An object that is an attribute of another object is embedded.

15.4 Instances as return values

Functions can return instances. For example, find_center takes a Rectangle as an argu- ment and returns a Point that contains the coordinates of the center of the Rectangle:

def find_center(rect):

p = Point() p.x = rect.corner.x + rect.width/2.0 p.y = rect.corner.y + rect.height/2.0 return p

Here is an example that passes box as an argument and assigns the resulting Point to center:

>>> center = find_center(box) >>> print_point(center) (50.0, 100.0)

15.5 Objects are mutable