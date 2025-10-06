,

a

’

’

’

,

c

f

’

’

’

,

]

b

’

’

,

d

’

’

]

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

,

’

f

’

]

If you omit the ﬁrst index, the slice starts at the beginning. If you omit the second, the slice goes to the end. So if you omit both, the slice is a copy of the whole list.

>>> t[:] ’ b , [

’

’

a

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

,

’

f

’

]

Since lists are mutable, it is often useful to make a copy before performing operations that fold, spindle or mutilate lists.

A slice operator on the left side of an assignment can update multiple elements:

’

’

>>> t = [ >>> t[1:3] = [ >>> print t [

,

a

’

’

’

’

’

a

,

x

,

y

’

’ ’

,

b x

’ ’

’

, ,

d

’

’ ’

,

c y

’ ’

’

, ]

e

’

’

,

d

’

’

,

f

’

’

]

e

’

,

’

f

’

]

10.6 List methods

Python provides methods that operate on lists. For example, append adds a new element to the end of a list: ’

’

’

’

’

’

a

>>> t = [ , >>> t.append( >>> print t [

b ’

,

c

]

’

d

)

’

’

’

’

’