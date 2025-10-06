def random_word(h):

t = [] for word, freq in h.items():

t.extend([word] * freq)

return random.choice(t)

The expression [word] * freq creates a list with freq copies of the string word. The extend method is similar to append except that the argument is a sequence. Exercise 13.7. This algorithm works, but it is not very efﬁcient; each time you choose a random word, it rebuilds the list, which is as big as the original book. An obvious improvement is to build the list once and then make multiple selections, but the list is still big.

An alternative is:

1. Use keys to get a list of the words in the book.

2. Build a list that contains the cumulative sum of the word frequencies (see Exercise 10.3). The last item in this list is the total number of words in the book, n.

3. Choose a random number from 1 to n. Use a bisection search (See Exercise 10.11) to ﬁnd the index where the random number would be inserted in the cumulative sum.