4. Use the index to ﬁnd the corresponding word in the word list.

Write a program that uses this algorithm to choose a random word from the book. Solution: http: //thinkpython.com/code/analyze_book3.py.

13.8 Markov analysis

If you choose words from the book at random, you can get a sense of the vocabulary, you probably won’t get a sentence:

this the small regard harriet which knightley

’

s it most things

A series of random words seldom makes sense because there is no relationship between successive words. For example, in a real sentence you would expect an article like “the” to be followed by an adjective or a noun, and probably not a verb or adverb.

One way to measure these kinds of relationships is Markov analysis, which characterizes, for a given sequence of words, the probability of the word that comes next. For example, the song Eric, the Half a Bee begins: