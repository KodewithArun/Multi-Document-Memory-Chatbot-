15.7 Debugging

When you start working with objects, you are likely to encounter some new exceptions. If you try to access an attribute that doesn’t exist, you get an AttributeError: >>> p = Point() >>> print p.z AttributeError: Point instance has no attribute

’

’

z

If you are not sure what type an object is, you can ask: >>> type(p) <type

’

’

__main__.Point

>

If you are not sure whether an object has a particular attribute, you can use the built-in function hasattr: ’ >>> hasattr(p, True >>> hasattr(p, False

’

)

x

’

’

z

)

15.8. Glossary

The ﬁrst argument can be any object; the second argument is a string that contains the name of the attribute.

15.8 Glossary

class: A user-deﬁned type. A class deﬁnition creates a new class object.

class object: An object that contains information about a user-deﬁned type. The class ob-

ject can be used to create instances of the type.

instance: An object that belongs to a class.