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

Other relational operations are useful for putting words in alphabetical order:

if word < print

’ ’

elif word > ’

print

’

banana Your word, banana : Your word,

:

’

’

’

’

+ word +

+ word +

’

’

, comes before banana.

, comes after banana.

’

’

else:

print

’

All right, bananas.

’

Python does not handle uppercase and lowercase letters the same way that people do. All the uppercase letters come before all the lowercase letters, so:

Your word, Pineapple, comes before banana.

A common way to address this problem is to convert strings to a standard format, such as all lowercase, before performing the comparison. Keep that in mind in case you have to defend yourself against a man armed with a Pineapple.

8.11 Debugging