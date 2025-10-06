Sort the list of tuples, and

Undecorate by extracting the sorted elements of the sequence.

For example, suppose you have a list of words and you want to sort them from longest to shortest: def sort_by_length(words):

t = [] for word in words:

t.append((len(word), word))

t.sort(reverse=True)

res = [] for length, word in t:

res.append(word)

return res

The ﬁrst loop builds a list of tuples, where each tuple is a word preceded by its length.

sort compares the ﬁrst element, length, ﬁrst, and only considers the second element to break ties. The keyword argument reverse=True tells sort to go in decreasing order.