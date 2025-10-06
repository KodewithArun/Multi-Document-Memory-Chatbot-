’

’

’

y

: 4,

: 3}

For purposes of debugging, you might ﬁnd it useful to keep this function handy: def print_attributes(obj):

for attr in obj.__dict__:

print attr, getattr(obj, attr)

print_attributes traverses the items in the object’s dictionary and prints each attribute name and its corresponding value.

The built-in function getattr takes an object and an attribute name (as a string) and returns the attribute’s value.

17.11 Interface and implementation

One of the goals of object-oriented design is to make software more maintainable, which means that you can keep the program working when other parts of the system change, and modify the program to meet new requirements.

A design principle that helps achieve that goal is to keep interfaces separate from imple- mentations. For objects, that means that the methods a class provides should not depend on how the attributes are represented.