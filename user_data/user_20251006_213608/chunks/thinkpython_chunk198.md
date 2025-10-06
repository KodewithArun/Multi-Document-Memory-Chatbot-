Solution: http://thinkpython.com/code/pi.py.

Chapter 8

Strings

8.1 A string is a sequence

A string is a sequence of characters. You can access the characters one at a time with the bracket operator:

’

’

>>> fruit = >>> letter = fruit[1]

banana

The second statement selects character number 1 from fruit and assigns it to letter.

The expression in brackets is called an index. The index indicates which character in the sequence you want (hence the name).

But you might not get what you expect:

>>> print letter a

’

’

For most people, the ﬁrst letter of index is an offset from the beginning of the string, and the offset of the ﬁrst letter is zero.

banana

is b, not a. But for computer scientists, the

>>> letter = fruit[0] >>> print letter b

So b is the 0th letter (“zero-eth”) of (“two-eth”) letter.

’

banana

’

, a is the 1th letter (“one-eth”), and n is the 2th