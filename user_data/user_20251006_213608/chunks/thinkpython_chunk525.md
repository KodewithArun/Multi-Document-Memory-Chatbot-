type

instantiate

obj

Figure C.6: Object diagram.

lumpy = Lumpy() lumpy.make_reference()

box = Rectangle() box.width = 100.0 box.height = 200.0 box.corner = Point() box.corner.x = 0.0 box.corner.y = 0.0

box2 = copy.copy(box)

lumpy.object_diagram()

Figure C.5 shows the result. copy.copy make a shallow copy, so box and box2 have their own width and height, but they share the same embedded Point object. This kind of sharing is usually ﬁne with immutable objects, but with mutable types, it is highly error- prone.

C.4 Function and class objects

When I use Lumpy to make object diagrams, I usually deﬁne the functions and classes before I make the reference point. That way, function and class objects don’t appear in the diagram.

215

216

Appendix C. Lumpy

object

Pointxy

Rectanglecornerheightwidth

Figure C.7: Class diagram.