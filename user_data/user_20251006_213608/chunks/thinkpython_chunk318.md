def different_words(hist):

return len(hist)

Here is some code to print the results:

print print

’ ’

’

Total number of words: Number of different words:

, total_words(hist)

’

, different_words(hist)

125

126

Chapter 13. Case study: data structure selection

And the results:

Total number of words: 161080 Number of different words: 7214

13.4 Most common words

To ﬁnd the most common words, we can apply the DSU pattern; most_common takes a histogram and returns a list of word-frequency tuples, sorted in reverse order by frequency:

def most_common(hist):

t = [] for key, value in hist.items(): t.append((value, key))

t.sort(reverse=True) return t

Here is a loop that prints the ten most common words:

t = most_common(hist) print for freq, word in t[0:10]: , freq

’

The most common words are:

’

’

print word,

\t

’

And here are the results from Emma: The most common words are: to the and of i a it her was she

5242

5205 4897

4295

3191 3130

2529

2483 2400 2364