’

’

oops

File "<stdin>", line 1, in ?

TypeError: list objects are unhashable

I mentioned earlier that a dictionary is implemented using a hashtable and that means that the keys have to be hashable.

A hash is a function that takes a value (of any kind) and returns an integer. Dictionaries use these integers, called hash values, to store and look up key-value pairs.

This system works ﬁne if the keys are immutable. But if the keys are mutable, like lists, bad things happen. For example, when you create a key-value pair, Python hashes the key and stores it in the corresponding location. If you modify the key and then hash it again, it would go to a different location. In that case you might have two entries for the same key, or you might not be able to ﬁnd a key. Either way, the dictionary wouldn’t work correctly.