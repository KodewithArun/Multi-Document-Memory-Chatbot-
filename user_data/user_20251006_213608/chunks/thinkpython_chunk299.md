Here the tuples are shown using Python syntax as a graphical shorthand.

The telephone number in the diagram is the complaints line for the BBC, so please don’t call it.

12.7 Comparing tuples

The relational operators work with tuples and other sequences; Python starts by comparing the ﬁrst element from each sequence. If they are equal, it goes on to the next elements, and so on, until it ﬁnds elements that differ. Subsequent elements are not considered (even if they are really big).

>>> (0, 1, 2) < (0, 3, 4) True >>> (0, 1, 2000000) < (0, 3, 4) True

The sort function works the same way. It sorts primarily by ﬁrst element, but in the case of a tie, it sorts by second element, and so on.

This feature lends itself to a pattern called DSU for

12.8. Sequences of sequences

Decorate a sequence by building a list of tuples with one or more sort keys preceding the

elements from the sequence,

Sort the list of tuples, and

Undecorate by extracting the sorted elements of the sequence.