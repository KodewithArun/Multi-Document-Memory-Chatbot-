Syntactically, a tuple is a comma-separated list of values: ’ d >>> t =

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

b

c

,

,

,

,

e

Although it is not necessary, it is common to enclose tuples in parentheses: ’ e >>> t = (

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

b

c

,

,

,

d

,

)

To create a tuple with a single element, you have to include a ﬁnal comma: >>> t1 = >>> type(t1) ’ tuple <type

’

’

a

,

’

>

A value in parentheses is not a tuple: >>> t2 = ( a >>> type(t2) ’ <type > Another way to create a tuple is the built-in function tuple. With no argument, it creates an empty tuple: >>> t = tuple() >>> print t ()

’

’

)

’

str

If the argument is a sequence (string, list or tuple), the result is a tuple with the elements of the sequence: >>> t = tuple( >>> print t ( Because tuple is the name of a built-in function, you should avoid using it as a variable name.

’

’

lupins

)

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

’

p

,

u

,

l

,

i

n

,

,

s

)