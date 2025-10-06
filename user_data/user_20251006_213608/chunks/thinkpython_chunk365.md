>>> center = find_center(box) >>> print_point(center) (50.0, 100.0)

15.5 Objects are mutable

You can change the state of an object by making an assignment to one of its attributes. For example, to change the size of a rectangle without changing its position, you can modify the values of width and height:

box.width = box.width + 50 box.height = box.width + 100

You can also write functions that modify objects. For example, grow_rectangle takes a Rectangle object and two numbers, dwidth and dheight, and adds the numbers to the width and height of the rectangle:

def grow_rectangle(rect, dwidth, dheight):

rect.width += dwidth rect.height += dheight

15.6. Copying

Here is an example that demonstrates the effect:

>>> print box.width 100.0 >>> print box.height 200.0 >>> grow_rectangle(box, 50, 100) >>> print box.width 150.0 >>> print box.height 300.0