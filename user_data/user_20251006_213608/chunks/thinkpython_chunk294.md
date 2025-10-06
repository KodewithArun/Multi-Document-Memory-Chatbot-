115

116

Chapter 12. Tuples

>>> max(1,2,3) 3

But sum does not.

>>> sum(1,2,3) TypeError: sum expected at most 2 arguments, got 3

Write a function called sumall that takes any number of arguments and returns their sum.

12.5 Lists and tuples

zip is a built-in function that takes two or more sequences and “zips” them into a list of tuples where each tuple contains one element from each sequence. In Python 3, zip returns an iterator of tuples, but for most purposes, an iterator behaves like a list.

This example zips a string and a list:

’

’

>>> s = >>> t = [0, 1, 2] >>> zip(s, t) ’ [(

abc

’

’

’

a

, 0), (

b

, 1), (

’

c

’

, 2)]

The result is a list of tuples where each tuple contains a character from the string and the corresponding element from the list.

If the sequences are not the same length, the result has the length of the shorter one.

>>> zip( ’ ’ A [(

’

,

’

E

’

Anne ’

), (

, ’

n

’ ’

Elk ’ ,

’

l

) ’

), (

’

n

’

,

’

k

’

)]