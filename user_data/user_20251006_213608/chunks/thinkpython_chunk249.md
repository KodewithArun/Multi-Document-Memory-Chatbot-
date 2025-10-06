10.11 Aliasing

If a refers to an object and you assign b = a, then both variables refer to the same object: >>> a = [1, 2, 3] >>> b = a >>> b is a True

The state diagram looks like Figure 10.4.

The association of a variable with an object is called a reference. In this example, there are two references to the same object.

An object with more than one reference has more than one name, so we say that the object is aliased.

If the aliased object is mutable, changes made with one alias affect the other:

10.12. List arguments

ab[ 1, 2, 3 ]

Figure 10.4: State diagram.

012’a’’b’’c’listtlettersdelete_head<module>

Figure 10.5: Stack diagram.

>>> b[0] = 17 >>> print a [17, 2, 3]

Although this behavior can be useful, it is error-prone. aliasing when you are working with mutable objects.

In general, it is safer to avoid

For immutable objects like strings, aliasing is not as much of a problem. In this example:

a = b =

’ ’

banana banana

’ ’