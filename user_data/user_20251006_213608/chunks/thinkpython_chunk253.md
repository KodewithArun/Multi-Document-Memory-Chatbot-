# WRONG!

Because sort returns None, the next operation you perform with t is likely to fail.

Before using list methods and operators, you should read the documentation care- fully and then test them in interactive mode. The methods and operators that lists share with other sequences (like strings) are documented at http://docs.python. org/2/library/stdtypes.html#typesseq. The methods and operators that only ap- ply to mutable sequences are documented at http://docs.python.org/2/library/ stdtypes.html#typesseq-mutable.

10.14. Glossary

2. Pick an idiom and stick with it.

Part of the problem with lists is that there are too many ways to do things. For exam- ple, to remove an element from a list, you can use pop, remove, del, or even a slice assignment.

To add an element, you can use the append method or the + operator. Assuming that t is a list and x is a list element, these are right:

t.append(x) t = t + [x]

And these are wrong:

t.append([x]) t = t.append(x) t + [x] t = t + x