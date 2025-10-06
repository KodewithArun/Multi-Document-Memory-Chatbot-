This is the ﬁrst example we have seen of a return statement inside a loop. If word[index] == letter, the function breaks out of the loop and returns immediately.

If the character doesn’t appear in the string, the program exits the loop normally and re- turns -1.

This pattern of computation—traversing a sequence and returning when we ﬁnd what we are looking for—is called a search. Exercise 8.4. Modify find so that it has a third parameter, the index in word where it should start looking.

8.7. Looping and counting

8.7 Looping and counting

The following program counts the number of times the letter a appears in a string:

’

’

word = count = 0 for letter in word: a if letter ==

banana

’

’

:

count = count + 1

print count