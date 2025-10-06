For the collection of sufﬁxes, the operations we need to perform include adding a new sufﬁx (or increasing the frequency of an existing one), and choosing a random sufﬁx.

Adding a new sufﬁx is equally easy for the list implementation or the histogram. Choosing a random element from a list is easy; choosing from a histogram is harder to do efﬁciently (see Exercise 13.7).

So far we have been talking mostly about ease of implementation, but there are other fac- tors to consider in choosing data structures. One is run time. Sometimes there is a theoreti- cal reason to expect one data structure to be faster than other; for example, I mentioned that the in operator is faster for dictionaries than for lists, at least when the number of elements is large.