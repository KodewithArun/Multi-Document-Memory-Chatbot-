13.9 Data structures

Using Markov analysis to generate random text is fun, but there is also a point to this exercise: data structure selection. In your solution to the previous exercises, you had to choose:

How to represent the preﬁxes.

129

130

Chapter 13. Case study: data structure selection

How to represent the collection of possible sufﬁxes.

How to represent the mapping from each preﬁx to the collection of possible sufﬁxes.

Ok, the last one is easy; the only mapping type we have seen is a dictionary, so it is the natural choice.

For the preﬁxes, the most obvious options are string, list of strings, or tuple of strings. For the sufﬁxes, one option is a list; another is a histogram (dictionary).