’

’ , ’ ’

’

>>> t = [ >>> delimiter = >>> delimiter.join(t) ’

pining

pining for the fjords

for

’

’

,

’

the

’

,

’

fjords

’

]

In this case the delimiter is a space character, so join puts a space between words. To concatenate strings without spaces, you can use the empty string,

’’

, as a delimiter.

10.10 Objects and values

If we execute these assignment statements:

a = b =

’ ’

banana banana

’ ’

We know that a and b both refer to a string, but we don’t know whether they refer to the same string. There are two possible states, shown in Figure 10.2.

In one case, a and b refer to two different objects that have the same value. In the second case, they refer to the same object.

To check whether two variables refer to the same object, you can use the is operator.

93

94

Chapter 10. Lists

ab’banana’ab’banana’’banana’

Figure 10.2: State diagram.

ab[ 1, 2, 3 ][ 1, 2, 3 ]

Figure 10.3: State diagram.

’ ’

>>> a = >>> b = >>> a is b True

banana banana

’ ’