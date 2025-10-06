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

’

’

’

a

c

,

,

b

,

d

]

extend takes a list as an argument and appends all of the elements:

’ ’

’ ’

’ ’

b >>> t1 = [ e >>> t2 = [ >>> t1.extend(t2) >>> print t1 ’ ’ [

a d

, ,

’

’

’

’

,

a

,

b

c

,

’

’ ’

d

, ]

’

,

’

c

’

’

e

]

’

]

This example leaves t2 unmodiﬁed.

sort arranges the elements of the list from low to high:

’

>>> t = [ >>> t.sort() >>> print t [

d

’

’

’

’

a

b

,

,

’

’

,

c

’

’

,

c

’

’

,

d

’

’

,

e

’

’

,

e

’

’

]

b

’

,

’

a

’

]

List methods are all void; they modify the list and return None. If you accidentally write t = t.sort(), you will be disappointed with the result.

10.7. Map, ﬁlter and reduce

10.7 Map, ﬁlter and reduce

To add up all the numbers in a list, you can use a loop like this:

def add_all(t):

total = 0 for x in t:

total += x

return total