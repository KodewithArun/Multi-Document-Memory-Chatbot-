’

banana

73

74

Chapter 8. Strings

An empty string contains no characters and has length 0, but other than that, it is the same as any other string. Exercise 8.3. Given that fruit is a string, what does fruit[:] mean?

8.5 Strings are immutable

It is tempting to use the [] operator on the left side of an assignment, with the intention of changing a character in a string. For example: >>> greeting = >>> greeting[0] = TypeError:

’

’

Hello, world!

’

’

J

’

’

str

object does not support item assignment

The “object” in this case is the string and the “item” is the character you tried to assign. For now, an object is the same thing as a value, but we will reﬁne that deﬁnition later. An item is one of the values in a sequence.