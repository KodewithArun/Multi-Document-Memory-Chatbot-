205

206

Appendix B. Analysis of Algorithms

Exercise B.3. Write a function called bisection that takes a sorted list and a target value and returns the index of the value in the list, if it’s there, or None if it’s not.

Or you could read the documentation of the bisect module and use that!

Bisection search can be much faster than linear search, but it requires the sequence to be in order, which might require extra work.

There is another data structure, called a hashtable that is even faster—it can do a search in constant time—and it doesn’t require the items to be sorted. Python dictionaries are implemented using hashtables, which is why most dictionary operations, including the in operator, are constant time.

B.4 Hashtables

To explain how hashtables work and why their performance is so good, I start with a simple implementation of a map and gradually improve it until it’s a hashtable.