The best kind of polymorphism is the unintentional kind, where you discover that a func- tion you already wrote can be applied to a type you never planned for.

163

164

Chapter 17. Classes and methods

17.10 Debugging

It is legal to add attributes to objects at any point in the execution of a program, but if you are a stickler for type theory, it is a dubious practice to have objects of the same type with different attribute sets. It is usually a good idea to initialize all of an object’s attributes in the init method.

If you are not sure whether an object has a particular attribute, you can use the built-in function hasattr (see Section 15.7).

Another way to access the attributes of an object is through the special attribute __dict__, which is a dictionary that maps attribute names (as strings) and values: >>> p = Point(3, 4) >>> print p.__dict__ ’ x {

’

’

’

y

: 4,

: 3}