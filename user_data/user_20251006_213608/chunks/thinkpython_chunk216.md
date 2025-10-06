invocation: A statement that calls a method.

8.13 Exercises

Exercise 8.10. A string slice can take a third index that speciﬁes the “step size;” that is, the number of spaces between successive characters. A step size of 2 means every other character; 3 means every third, etc.

’

>>> fruit = >>> fruit[0:5:2] ’

banana

’

bnn

’

A step size of -1 goes through the word backwards, so the slice [::-1] generates a reversed string.

Use this idiom to write a one-line version of is_palindrome from Exercise 6.6. Exercise 8.11. The following functions are all intended to check whether a string contains any lowercase letters, but at least some of them are wrong. For each function, describe what the function actually does (assuming that the parameter is a string).

def any_lowercase1(s):

for c in s:

if c.islower(): return True

else:

return False

def any_lowercase2(s):

for c in s: if

’

’

c return

.islower(): ’ ’

True

79

80

Chapter 8. Strings

else:

return

’

False

’