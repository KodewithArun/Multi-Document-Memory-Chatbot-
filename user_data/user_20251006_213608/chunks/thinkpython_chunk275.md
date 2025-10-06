That’s why the keys have to be hashable, and why mutable types like lists aren’t. The simplest way to get around this limitation is to use tuples, which we will see in the next chapter.

Since lists and dictionaries are mutable, they can’t be used as keys, but they can be used as values. Exercise 11.5. Read the documentation of the dictionary method setdefault and use it to write a more concise version of invert_dict. Solution: http://thinkpython.com/code/invert_ dict.py.

11.5 Memos

If you played with the fibonacci function from Section 6.7, you might have noticed that the bigger the argument you provide, the longer the function takes to run. Furthermore,

11.5. Memos

fibonaccin4fibonaccin3fibonaccin2fibonaccin0fibonaccin1fibonaccin1fibonaccin2fibonaccin0fibonaccin1

Figure 11.2: Call graph.

the run time increases very quickly.

To understand why, consider Figure 11.2, which shows the call graph for fibonacci with n=4: