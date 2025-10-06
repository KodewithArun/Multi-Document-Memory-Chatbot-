def histogram(s): d = dict() for c in s:

if c not in d:

d[c] = 1

else:

d[c] = d[c]+1

return d

This function also works for lists, tuples, and even dictionaries, as long as the elements of s are hashable, so they can be used as keys in d.

’

’

>>> t = [ , >>> histogram(t) ’ {

spam

’

’

: 1,

bacon

egg

’

’

egg

’

: 1,

,

’

’

spam

spam

’

’

,

’

: 4}

spam

’

,

’

bacon

’

,

’

spam

’

]

Functions that can work with several types are called polymorphic. Polymorphism can facilitate code reuse. For example, the built-in function sum, which adds the elements of a sequence, works as long as the elements of the sequence support addition.

Since Time objects provide an add method, they work with sum:

>>> t1 = Time(7, 43) >>> t2 = Time(7, 41) >>> t3 = Time(7, 37) >>> total = sum([t1, t2, t3]) >>> print total 23:01:00

In general, if all of the operations inside a function work with a given type, then the func- tion works with that type.