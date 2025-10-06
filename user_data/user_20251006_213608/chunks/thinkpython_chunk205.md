The reason for the error is that strings are immutable, which means you can’t change an existing string. The best you can do is create a new string that is a variation on the original: >>> greeting = >>> new_greeting = >>> print new_greeting Jello, world! This example concatenates a new ﬁrst letter onto a slice of greeting. It has no effect on the original string.

’

’

Hello, world!

’

’

J

+ greeting[1:]

8.6 Searching

What does the following function do? def find(word, letter):

index = 0 while index < len(word):

if word[index] == letter:

return index

index = index + 1

return -1

In a sense, find is the opposite of the [] operator. Instead of taking an index and extracting the corresponding character, it takes a character and ﬁnds the index where that character appears. If the character is not found, the function returns -1.