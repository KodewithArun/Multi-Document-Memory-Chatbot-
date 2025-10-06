8.11 Debugging

When you use indices to traverse the values in a sequence, it is tricky to get the beginning and end of the traversal right. Here is a function that is supposed to compare two words and return True if one of the words is the reverse of the other, but it contains two errors:

def is_reverse(word1, word2):

if len(word1) != len(word2):

return False

i = 0 j = len(word2)

while j > 0:

if word1[i] != word2[j]:

return False

i = i+1 j = j-1

return True

The ﬁrst if statement checks whether the words are the same length. If not, we can return False immediately and then, for the rest of the function, we can assume that the words are the same length. This is an example of the guardian pattern in Section 6.8.

i and j are indices: i traverses word1 forward while j traverses word2 backward. If we ﬁnd two letters that don’t match, we can return False immediately. If we get through the whole loop and all the letters match, we return True.