def add_all(t):

total = 0 for x in t:

total += x

return total

total is initialized to 0. Each time through the loop, x gets one element from the list. The += operator provides a short way to update a variable. This augmented assignment statement:

total += x

is equivalent to:

total = total + x

As the loop executes, total accumulates the sum of the elements; a variable used this way is sometimes called an accumulator.

Adding up the elements of a list is such a common operation that Python provides it as a built-in function, sum:

>>> t = [1, 2, 3] >>> sum(t) 6

An operation like this that combines a sequence of elements into a single value is some- times called reduce. Exercise 10.1. Write a function called nested_sum that takes a nested list of integers and add up the elements from all of the nested lists.