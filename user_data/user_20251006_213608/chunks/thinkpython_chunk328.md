How should you choose? The ﬁrst step is to think about the operations you will need to implement for each data structure. For the preﬁxes, we need to be able to remove words from the beginning and add to the end. For example, if the current preﬁx is “Half a,” and the next word is “bee,” you need to be able to form the next preﬁx, “a bee.”

Your ﬁrst choice might be a list, since it is easy to add and remove elements, but we also need to be able to use the preﬁxes as keys in a dictionary, so that rules out lists. With tuples, you can’t append or remove, but you can use the addition operator to form a new tuple: def shift(prefix, word):

return prefix[1:] + (word,)

shift takes a tuple of words, prefix, and a string, word, and forms a new tuple that has all the words in prefix except the ﬁrst, and word added to the end.