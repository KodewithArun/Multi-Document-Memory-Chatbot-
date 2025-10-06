’

banana

’

, a is the 1th letter (“one-eth”), and n is the 2th

You can use any expression, including variables and operators, as an index, but the value of the index has to be an integer. Otherwise you get:

>>> letter = fruit[1.5] TypeError: string indices must be integers, not float

8.2 len

len is a built-in function that returns the number of characters in a string:

72

Chapter 8. Strings

’

>>> fruit = >>> len(fruit) 6

banana

’

To get the last letter of a string, you might be tempted to try something like this:

>>> length = len(fruit) >>> last = fruit[length] IndexError: string index out of range

The reason for the IndexError is that there is no letter in ’banana’ with the index 6. Since we started counting at zero, the six letters are numbered 0 to 5. To get the last character, you have to subtract 1 from length:

>>> last = fruit[length-1] >>> print last a