tres

two

uno

}

’

’

’

’

’

’

’

’

’

’

:

two

tres

,

,

uno

three

:

:

one

}

dos

The order of the key-value pairs is not the same. In fact, if you type the same example on your computer, you might get a different result. In general, the order of items in a dictionary is unpredictable.

But that’s not a problem because the elements of a dictionary are never indexed with inte- ger indices. Instead, you use the keys to look up the corresponding values:

102

Chapter 11. Dictionaries

>>> print eng2sp[ ’

’

dos

’

two

’

]

The key ’two’ always maps to the value

’

dos

’

so the order of the items doesn’t matter.

If the key isn’t in the dictionary, you get an exception: ’

’

four

>>> print eng2sp[ KeyError:

]

’

’

four

The len function works on dictionaries; it returns the number of key-value pairs:

>>> len(eng2sp) 3