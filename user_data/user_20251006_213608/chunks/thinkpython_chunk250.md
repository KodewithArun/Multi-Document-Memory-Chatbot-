a = b =

’ ’

banana banana

’ ’

It almost never makes a difference whether a and b refer to the same string or not.

10.12 List arguments

When you pass a list to a function, the function gets a reference to the list. If the function modiﬁes a list parameter, the caller sees the change. For example, delete_head removes the ﬁrst element from a list:

def delete_head(t):

del t[0]

Here’s how it is used: ’

’

’

, >>> letters = [ >>> delete_head(letters) >>> print letters ’ [

a

,

b

’

’

’

b

,

c

]

’

’

c

’

]

The parameter t and the variable letters are aliases for the same object. The stack diagram looks like Figure 10.5.

Since the list is shared by two frames, I drew it between them.

It is important to distinguish between operations that modify lists and operations that cre- ate new lists. For example, the append method modiﬁes a list, but the + operator creates a new list:

>>> t1 = [1, 2] >>> t2 = t1.append(3)

95

96

Chapter 10. Lists