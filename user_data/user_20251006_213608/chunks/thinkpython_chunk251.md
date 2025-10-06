>>> t1 = [1, 2] >>> t2 = t1.append(3)

95

96

Chapter 10. Lists

>>> print t1 [1, 2, 3] >>> print t2 None

>>> t3 = t1 + [4] >>> print t3 [1, 2, 3, 4]

This difference is important when you write functions that are supposed to modify lists. For example, this function does not delete the head of a list:

def bad_delete_head(t):

t = t[1:]

# WRONG!

The slice operator creates a new list and the assignment makes t refer to it, but none of that has any effect on the list that was passed as an argument.

An alternative is to write a function that creates and returns a new list. For example, tail returns all but the ﬁrst element of a list:

def tail(t):

return t[1:]

This function leaves the original list unmodiﬁed. Here’s how it is used:

’

’

’

>>> letters = [ , >>> rest = tail(letters) >>> print rest ’ c [

,

a

b

’

’

’

b

,

]

’

’

c

’

]

10.13 Debugging