Here’s how it works: >>> h = histogram( >>> print h { : 2, b : 1, The histogram indicates that the letters ’a’ and so on. Exercise 11.2. Dictionaries have a method called get that takes a key and a default value. If the key appears in the dictionary, get returns the corresponding value; otherwise it returns the default value. For example: >>> h = histogram( >>> print h { : 1} >>> h.get( 1 >>> h.get( 0 Use get to write histogram more concisely. You should be able to eliminate the if statement.

’

’

brontosaurus

)

’

’

’

’

’

’

’ : 2, : 2, u ’ appear once;

’

’

’

’

’

’

’ r ’ b

’ t ’ o

’ ’

s

: 1} appears twice, and

: 2,

: 1,

a

: 1,

n

o

’

’

a

)

’

’

a

’

’

a

, 0)

’

’

, 0)

b

11.2 Looping and dictionaries

If you use a dictionary in a for statement, it traverses the keys of the dictionary. For exam- ple, print_hist prints each key and the corresponding value:

104

Chapter 11. Dictionaries

def print_hist(h): for c in h:

print c, h[c]