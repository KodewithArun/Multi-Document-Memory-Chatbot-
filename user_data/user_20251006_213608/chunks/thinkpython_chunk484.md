Second, clean up the program. Remove dead code and reorganize the program to make it as easy to read as possible. For example, if you suspect that the problem is in a deeply nested part of the program, try rewriting that part with simpler structure. If you suspect a large function, try splitting it into smaller functions and testing them separately.

Often the process of ﬁnding the minimal test case leads you to the bug. If you ﬁnd that a program works in one situation but not in another, that gives you a clue about what is going on.

Similarly, rewriting a piece of code can help you ﬁnd subtle bugs. If you make a change that you think shouldn’t affect the program, and it does, that can tip you off.

A.3 Semantic errors

In some ways, semantic errors are the hardest to debug, because the interpreter provides no information about what is wrong. Only you know what the program is supposed to do.