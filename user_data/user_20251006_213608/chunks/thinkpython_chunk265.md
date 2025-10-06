>>> vals = eng2sp.values() >>> in vals True

’

’

uno

The in operator uses different algorithms for lists and dictionaries. For lists, it uses a search algorithm, as in Section 8.6. As the list gets longer, the search time gets longer in direct proportion. For dictionaries, Python uses an algorithm called a hashtable that has a re- markable property: the in operator takes about the same amount of time no matter how many items there are in a dictionary. I won’t explain how that’s possible, but you can read more about it at http://en.wikipedia.org/wiki/Hash_table. Exercise 11.1. Write a function that reads the words in words.txt and stores them as keys in a dictionary. It doesn’t matter what the values are. Then you can use the in operator as a fast way to check whether a string is in the dictionary.

If you did Exercise 10.11, you can compare the speed of this implementation with the list in operator and the bisection search.

11.1 Dictionary as a set of counters