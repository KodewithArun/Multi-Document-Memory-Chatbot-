The second loop traverses the list of tuples and builds a list of words in descending order of length. Exercise 12.2. In this example, ties are broken by comparing words, so words with the same length appear in reverse alphabetical order. For other applications you might want to break ties at ran- dom. Modify this example so that words with the same length appear in random order. Hint: see the random function in the random module. Solution: http://thinkpython.com/code/ unstable_sort.py.

12.8 Sequences of sequences

I have focused on lists of tuples, but almost all of the examples in this chapter also work with lists of lists, tuples of tuples, and tuples of lists. To avoid enumerating the possible combinations, it is sometimes easier to talk about sequences of sequences.

In many contexts, the different kinds of sequences (strings, lists and tuples) can be used interchangeably. So how and why do you choose one over the others?