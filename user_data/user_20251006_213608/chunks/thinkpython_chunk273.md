Here is an example:

’

’

parrot

>>> hist = histogram( >>> print hist { >>> inverse = invert_dict(hist) >>> print inverse t , {1: [

)

’

’

’

’

’

’

’

’

p

: 1,

r

t

: 2,

: 1,

a

: 1,

’

’

’

’

’

’

’

’

’

a

p

], 2: [

o

,

,

r

’

’

o

]}

’

: 1}

105

106

Chapter 11. Dictionaries

’a’11dicthist’p’1’o’1’r’2’t’01’a’’p’list2’t’’o’31dictinv20list’r’

Figure 11.1: State diagram.

Figure 11.1 is a state diagram showing hist and inverse. A dictionary is represented as a box with the type dict above it and the key-value pairs inside. If the values are integers, ﬂoats or strings, I usually draw them inside the box, but I usually draw lists outside the box, just to keep the diagram simple.

Lists can be values in a dictionary, as this example shows, but they cannot be keys. Here’s what happens if you try: >>> t = [1, 2, 3] >>> d = dict() >>> d[t] = Traceback (most recent call last):

’

’

oops

File "<stdin>", line 1, in ?

TypeError: list objects are unhashable