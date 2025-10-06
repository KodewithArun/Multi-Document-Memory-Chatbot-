>>> print absolute_value(0) None

By the way, Python provides a built-in function called abs that computes absolute values. Exercise 6.1. Write a compare function that returns 1 if x > y, 0 if x == y, and -1 if x < y.

6.2 Incremental development

As you write larger functions, you might ﬁnd yourself spending more time debugging.

To deal with increasingly complex programs, you might want to try a process called in- cremental development. The goal of incremental development is to avoid long debugging sessions by adding and testing only a small amount of code at a time.

As an example, suppose you want to ﬁnd the distance between two points, given by the coordinates (x1,y1) and (x2,y2). By the Pythagorean theorem, the distance is:

distance =

(cid:113)

(x2 − x1)2 + (y2 − y1)2

The ﬁrst step is to consider what a distance function should look like in Python. In other words, what are the inputs (parameters) and what is the output (return value)?