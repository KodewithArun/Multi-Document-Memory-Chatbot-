Removing an element from the end of a list is constant time.

Sorting is O(nlogn).

Most dictionary operations and methods are constant time, but there are some exceptions:

The run time of copy is proportional to the number of elements, but not the size of the elements (it copies references, not the elements themselves).

B.3. Analysis of search algorithms

The run time of update is proportional to the size of the dictionary passed as a pa- rameter, not the dictionary being updated.

keys, values and items are linear because they return new lists; iterkeys, itervalues and iteritems are constant time because they return iterators. But if you loop through the iterators, the loop will be linear. Using the “iter” functions saves some overhead, but it doesn’t change the order of growth unless the number of items you access is bounded.