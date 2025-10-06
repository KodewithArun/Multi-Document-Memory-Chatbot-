pend on its implementation, in particular the representation of its attributes.

17.13 Exercises

Exercise 17.7. This exercise is a cautionary tale about one of the most common, and difﬁcult to ﬁnd, errors in Python. Write a deﬁnition for a class named Kangaroo with the following methods:

1. An __init__ method that initializes an attribute named pouch_contents to an empty list.

2. A method named put_in_pouch that takes an object of any type and adds it to pouch_contents.

3. A __str__ method that returns a string representation of the Kangaroo object and the con- tents of the pouch.

Test your code by creating two Kangaroo objects, assigning them to variables named kanga and roo, and then adding roo to the contents of kanga’s pouch.

165

166

Chapter 17. Classes and methods

Download http://thinkpython.com/code/BadKangaroo.py. It contains a solution to the previous problem with one big, nasty bug. Find and ﬁx the bug.