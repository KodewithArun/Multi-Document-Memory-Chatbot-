10.8 Deleting elements

There are several ways to delete elements from a list. If you know the index of the element you want, you can use pop: ’ ’ ] b a >>> t = [ >>> x = t.pop(1) >>> print t [ >>> print x b pop modiﬁes the list and returns the element that was removed. If you don’t provide an index, it deletes and returns the last element.

’

’

’

’

c

,

,

’

’

’

’

c

,

a

]

If you don’t need the removed value, you can use the del operator: >>> t = [ >>> del t[1] >>> print t [ If you know the element you want to remove (but not the index), you can use remove: >>> t = [ , >>> t.remove( >>> print t [ The return value from remove is None.

’

’

’

’

’

’

a

,

c

b

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