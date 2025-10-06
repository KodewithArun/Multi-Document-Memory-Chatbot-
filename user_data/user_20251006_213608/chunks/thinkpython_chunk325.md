In this example the length of the preﬁx is always two, but you can do Markov analysis with any preﬁx length. The length of the preﬁx is called the “order” of the analysis. Exercise 13.8. Markov analysis:

1. Write a program to read a text from a ﬁle and perform Markov analysis. The result should be a dictionary that maps from preﬁxes to a collection of possible sufﬁxes. The collection might be a list, tuple, or dictionary; it is up to you to make an appropriate choice. You can test your program with preﬁx length two, but you should write the program in a way that makes it easy to try other lengths.

2. Add a function to the previous program to generate random text based on the Markov analysis. Here is an example from Emma with preﬁx length 2:

He was very clever, be it sweetness or be angry, ashamed or only amused, at such a stroke. She had never thought of Hannah till you were never meant for me?" "I cannot make speeches, Emma:" he soon cut it all himself.