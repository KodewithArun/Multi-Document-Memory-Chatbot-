Chapter 13

Case study: data structure selection

13.1 Word frequency analysis

As usual, you should at least attempt the following exercises before you read my solutions. Exercise 13.1. Write a program that reads a ﬁle, breaks each line into words, strips whitespace and punctuation from the words, and converts them to lowercase.

Hint: The string module provides strings named whitespace, which contains space, tab, newline, etc., and punctuation which contains the punctuation characters. Let’s see if we can make Python swear:

>>> import string >>> print string.punctuation ‘ !"#$%&

’

()*+,-./:;<=>?@[\]^_

{|}~

Also, you might consider using the string methods strip, replace and translate. Exercise 13.2. Go to Project Gutenberg (http://gutenberg.org) and download your favorite out-of-copyright book in plain text format.