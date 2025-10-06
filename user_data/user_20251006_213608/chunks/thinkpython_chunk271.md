File "<stdin>", line 1, in ? File "<stdin>", line 5, in reverse_lookup

ValueError

The result when you raise an exception is the same as when Python raises one: it prints a traceback and an error message.

The raise statement takes a detailed error message as an optional argument. For example:

’

>>> raise ValueError( Traceback (most recent call last):

value does not appear in the dictionary

’

)

File "<stdin>", line 1, in ?

ValueError: value does not appear in the dictionary

A reverse lookup is much slower than a forward lookup; if you have to do it often, or if the dictionary gets big, the performance of your program will suffer. Exercise 11.4. Modify reverse_lookup so that it builds and returns a list of all keys that map to v, or an empty list if there are none.

11.4 Dictionaries and lists