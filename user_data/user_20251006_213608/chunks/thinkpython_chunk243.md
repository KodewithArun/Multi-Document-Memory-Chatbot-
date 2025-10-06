def only_upper(t):

res = [] for s in t:

91

92

Chapter 10. Lists

if s.isupper():

res.append(s)

return res

isupper is a string method that returns True if the string contains only upper case letters.

An operation like only_upper is called a ﬁlter because it selects some of the elements and ﬁlters out the others.

Most common list operations can be expressed as a combination of map, ﬁlter and reduce. Because these operations are so common, Python provides language features to support them, including the built-in function map and an operator called a “list comprehension.” Exercise 10.3. Write a function that takes a list of numbers and returns the cumulative sum; that is, a new list where the ith element is the sum of the ﬁrst i + 1 elements from the original list. For example, the cumulative sum of [1, 2, 3] is [1, 3, 6].

10.8 Deleting elements