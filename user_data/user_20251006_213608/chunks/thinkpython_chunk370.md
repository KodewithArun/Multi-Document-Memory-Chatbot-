ject can be used to create instances of the type.

instance: An object that belongs to a class.

attribute: One of the named values associated with an object.

embedded (object): An object that is stored as an attribute of another object.

shallow copy: To copy the contents of an object, including any references to embedded

objects; implemented by the copy function in the copy module.

deep copy: To copy the contents of an object as well as any embedded objects, and any objects embedded in them, and so on; implemented by the deepcopy function in the copy module.

object diagram: A diagram that shows objects, their attributes, and the values of the at-

tributes.

15.9 Exercises

Exercise 15.4. Swampy (see Chapter 4) provides a module named World, which deﬁnes a user- deﬁned type also called World. You can import it like this: from swampy.World import World

Or, depending on how you installed Swampy, like this: from World import World