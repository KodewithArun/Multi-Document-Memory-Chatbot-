]

,

’

’

’

’

c

,

]

a

’

’

’

’

’

’

,

b ’

a

c

]

’

b

)

’

’

’

’

,

]

a

c

To remove more than one element, you can use del with a slice index: ’ >>> t = [ >>> del t[1:5] >>> print t [ As usual, the slice selects all the elements up to, but not including, the second index. Exercise 10.4. Write a function called middle that takes a list and returns a new list that contains all but the ﬁrst and last elements. So middle([1,2,3,4]) should return [2,3]. Exercise 10.5. Write a function called chop that takes a list, modiﬁes it by removing the ﬁrst and last elements, and returns None.

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

c

b

a

,

d

,

,

,

,

e

f

]

’

’

’

’

]

a

,

f

10.9. Lists and strings

10.9 Lists and strings

A string is a sequence of characters and a list is a sequence of values, but a list of characters is not the same as a string. To convert from a string to a list of characters, you can use list:

’

’

>>> s = >>> t = list(s) >>> print t [

spam