A for loop over an empty list never executes the body:

for x in []: print

’

This never happens.

’

Although a list can contain another list, the nested list still counts as a single element. The length of this list is four:

[

’

spam

’

, 1, [

’

Brie

’

,

’

Roquefort

’

,

’

Pol le Veq

’

], [1, 2, 3]]

10.4 List operations

The + operator concatenates lists:

>>> a = [1, 2, 3] >>> b = [4, 5, 6] >>> c = a + b >>> print c [1, 2, 3, 4, 5, 6]

Similarly, the * operator repeats a list a given number of times:

>>> [0] * 4 [0, 0, 0, 0] >>> [1, 2, 3] * 3 [1, 2, 3, 1, 2, 3, 1, 2, 3]

The ﬁrst example repeats [0] four times. The second example repeats the list [1, 2, 3] three times.

10.5 List slices

The slice operator also works on lists:

89

90

Chapter 10. Lists

>>> t = [ >>> t[1:3] [ ] , >>> t[:4] ’ [ , >>> t[3:] ’ , [

’

’

’

’

c

b

’

’

’

a

b

’

’

’

d

e

’

,

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