Here is a function that takes a value and returns the ﬁrst key that maps to that value:

def reverse_lookup(d, v):

for k in d:

if d[k] == v:

return k raise ValueError

This function is yet another example of the search pattern, but it uses a feature we haven’t seen before, raise. The raise statement causes an exception; in this case it causes a ValueError, which generally indicates that there is something wrong with the value of a parameter.

If we get to the end of the loop, that means v doesn’t appear in the dictionary as a value, so we raise an exception.

Here is an example of a successful reverse lookup:

’

’

>>> h = histogram( >>> k = reverse_lookup(h, 2) >>> print k r

parrot

)

And an unsuccessful one:

11.4. Dictionaries and lists

>>> k = reverse_lookup(h, 3) Traceback (most recent call last):

File "<stdin>", line 1, in ? File "<stdin>", line 5, in reverse_lookup

ValueError