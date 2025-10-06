7. Many of the non-comparison sorts are linear, so why does does Python use an O(nlogn) comparison sort?

B.3 Analysis of search algorithms

A search is an algorithm that takes a collection and a target item and determines whether the target is in the collection, often returning the index of the target.

The simplest search algorithm is a “linear search,” which traverses the items of the collec- tion in order, stopping if it ﬁnds the target. In the worst case it has to traverse the entire collection, so the run time is linear.

The in operator for sequences uses a linear search; so do string methods like find and count.