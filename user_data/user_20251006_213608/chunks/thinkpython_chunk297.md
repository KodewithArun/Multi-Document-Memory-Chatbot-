’

’

’

’

a

: 2,

’

’

abc

’

, range(3)))

b

’

: 1}

The dictionary method update also takes a list of tuples and adds them, as key-value pairs, to an existing dictionary.

Combining items, tuple assignment and for, you get the idiom for traversing the keys and values of a dictionary:

for key, val in d.items():

print val, key

The output of this loop is:

0 a 2 c 1 b

Again.

It is common to use tuples as keys in dictionaries (primarily because you can’t use lists). For example, a telephone directory might map from last-name, ﬁrst-name pairs to telephone numbers. Assuming that we have deﬁned last, first and number, we could write:

directory[last,first] = number

The expression in brackets is a tuple. We could use tuple assignment to traverse this dic- tionary.

117

118

Chapter 12. Tuples

01’Cleese’’John’tuple

Figure 12.1: State diagram.