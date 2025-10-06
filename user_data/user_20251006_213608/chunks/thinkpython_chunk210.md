a

syntax that might

be

confusing.

For

example,

8.9 The in operator

The word in is a boolean operator that takes two strings and returns True if the ﬁrst ap- pears as a substring in the second:

’

>>> True >>> False

’

a

’

in

seed

’

’

banana

’

in

’

banana

’

For example, the following function prints all the letters from word1 that also appear in word2: def in_both(word1, word2):

for letter in word1:

if letter in word2: print letter

With well-chosen variable names, Python sometimes reads like English. You could read this loop, “for (each) letter in (the ﬁrst) word, if (the) letter (appears) in (the second) word, print (the) letter.”

Here’s what you get if you compare apples and oranges:

>>> in_both( a e s

’

apples

’

,

’

oranges

’

)

8.10 String comparison

The relational operators work on strings. To see if two strings are equal:

8.11. Debugging

if word ==

print

’

’

banana

’

:

All right, bananas.

’