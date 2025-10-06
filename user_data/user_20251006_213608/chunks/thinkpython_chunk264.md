>>> len(eng2sp) 3

The in operator works on dictionaries; it tells you whether something appears as a key in the dictionary (appearing as a value is not good enough).

’

>>> True >>> False

’

one

uno

’

’

in eng2sp

in eng2sp

To see whether something appears as a value in a dictionary, you can use the method values, which returns the values as a list, and then use the in operator:

>>> vals = eng2sp.values() >>> in vals True

’

’

uno