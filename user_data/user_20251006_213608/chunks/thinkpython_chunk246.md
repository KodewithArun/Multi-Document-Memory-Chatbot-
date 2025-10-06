’

’

>>> s = >>> t = list(s) >>> print t [

spam

’

’

’

’

’

’

s

,

p

,

a

,

’

m

’

]

Because list is the name of a built-in function, you should avoid using it as a variable name. I also avoid l because it looks too much like 1. So that’s why I use t.

The list function breaks a string into individual letters. If you want to break a string into words, you can use the split method:

’

’

pining for the fjords

>>> s = >>> t = s.split() >>> print t pining [

’

’

’

’

’

’

’

for

the

,

,

,

fjords

’

]

An optional argument called a delimiter speciﬁes which characters to use as word bound- aries. The following example uses a hyphen as a delimiter:

’

>>> s = >>> delimiter = >>> s.split(delimiter) spam [

spam-spam-spam ’

’



’

’

’

’

’

,

spam

,

spam

’

’

]

join is the inverse of split. It takes a list of strings and concatenates the elements. join is a string method, so you have to invoke it on the delimiter and pass the list as a parameter:

’