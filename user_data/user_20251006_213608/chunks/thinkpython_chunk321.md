’

t in the word list are:

rencontre jane

s blanche woodhouses disingenuousness

’

friend Some of these words are names and possessives. Others, like “rencontre,” are no longer in common use. But a few are common words that should really be in the list! Exercise 13.6. Python provides a data structure called set that provides many common set opera- tions. Read the documentation at http://docs.python.org/2/library/stdtypes.html# types-set and write a program that uses set subtraction to ﬁnd words in the book that are not in the word list. Solution: http://thinkpython.com/code/analyze_book2.py.

s venice apartment ...

13.7 Random words

To choose a random word from the histogram, the simplest algorithm is to build a list with multiple copies of each word, according to the observed frequency, and then choose from the list:

127

128

Chapter 13. Case study: data structure selection

def random_word(h):

t = [] for word, freq in h.items():

t.extend([word] * freq)