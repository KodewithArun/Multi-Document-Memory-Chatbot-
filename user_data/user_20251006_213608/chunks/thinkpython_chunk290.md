’

’

lupins

)

’

’

’

’

’

’

’

’

’

’

’

’

p

,

u

,

l

,

i

n

,

,

s

)

Most list operators also work on tuples. The bracket operator indexes an element:

114

Chapter 12. Tuples

’

’

a

>>> t = ( >>> print t[0] ’

,

’

a

’

b

’

,

’

c

’

,

’

d

’

,

’

e

’

)

And the slice operator selects a range of elements.

>>> print t[1:3] ’ c (

’

’

’

b

,

)

But if you try to modify one of the elements of the tuple, you get an error:

’

’

>>> t[0] = TypeError: object doesn

A

’

t support item assignment

You can’t modify the elements of a tuple, but you can replace one tuple with another:

’

>>> t = ( A >>> print t (

’

’

’

’

,

A

b

,

’

’

,) + t[1:]

c

’

,

’

d

’

,

’

e

’

)

12.2 Tuple assignment

It is often useful to swap the values of two variables. With conventional assignments, you have to use a temporary variable. For example, to swap a and b:

>>> temp = a >>> a = b >>> b = temp