The ﬁle object keeps track of where it is in the ﬁle, so if you call readline again, you get the next word: >>> fin.readline() ’ ’

aah\r\n

The next word is “aah,” which is a perfectly legitimate word, so stop looking at me like that. Or, if it’s the whitespace that’s bothering you, we can get rid of it with the string method strip:

82

Chapter 9. Case study: word play

>>> line = fin.readline() >>> word = line.strip() >>> print word aahed You can also use a ﬁle object as part of a for loop. This program reads words.txt and prints each word, one per line: fin = open( for line in fin:

’

’

words.txt

)

word = line.strip() print word

Exercise 9.1. Write a program that reads words.txt and prints only the words with more than 20 characters (not counting whitespace).

9.2 Exercises