’

abc

’

):

print index, element

12.6. Dictionaries and tuples

The output of this loop is:

0 a 1 b 2 c

Again.

12.6 Dictionaries and tuples

Dictionaries have a method called items that returns a list of tuples, where each tuple is a key-value pair. ’

’

’

’

’

’

b

:0,

:1,

c

a

:2}

>>> d = { >>> t = d.items() >>> print t [(

’

’

’

’

’

’

, 0), (

, 2), (

c

a

b

, 1)]

As you should expect from a dictionary, the items are in no particular order. In Python 3, items returns an iterator, but for many purposes, iterators behave like lists.

Going in the other direction, you can use a list of tuples to initialize a new dictionary:

’

’

a

>>> t = [( >>> d = dict(t) >>> print d c : 0, {

, 0), (

’

’

’

’

’

’

a

: 2,

b

’

c

’

, 2), (

: 1}

’

b

’

, 1)]

Combining dict with zip yields a concise way to create a dictionary:

>>> d = dict(zip( >>> print d c : 0, {

’

’

’

’

a

: 2,

’

’

abc

’

, range(3)))

b

’

: 1}