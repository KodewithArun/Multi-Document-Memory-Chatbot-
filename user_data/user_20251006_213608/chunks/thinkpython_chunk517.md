An important feature of this algorithm is that when we resize the HashTable it grows geometrically; that is, we multiply the size by a constant. If you increase the size arithmetically—adding a ﬁxed number each time—the average time per add is linear.

You can download my implementation of HashMap from http://thinkpython/code/ Map.py, but remember that there is no reason to use it; if you want a map, just use a Python dictionary.

209

210

Appendix B. Analysis of Algorithms

Appendix C

Lumpy

Throughout the book, I have used diagrams to represent the state of running programs.

In Section 2.2, we used a state diagram to show the names and values of variables. In Section 3.10 I introduced a stack diagram, which shows one frame for each function call. Each frame shows the parameters and local variables for the function or method. Stack diagrams for recursive functions appear in Section 5.9 and Section 6.5.