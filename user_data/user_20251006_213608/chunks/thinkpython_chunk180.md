 



n + 1 A(m − 1,1) A(m − 1, A(m,n − 1))

if m = 0 if m > 0 and n = 0 if m > 0 and n > 0.

See http://en.wikipedia.org/wiki/Ackermann_function. Write a function named ack that evaluates Ackermann’s function. Use your function to evaluate ack(3, 4), which should be 125. What happens for larger values of m and n? Solution: http://thinkpython.com/code/ ackermann.py. Exercise 6.6. A palindrome is a word that is spelled the same backward and forward, like “noon” and “redivider”. Recursively, a word is a palindrome if the ﬁrst and last letters are the same and the middle is a palindrome.

The following are functions that take a string argument and return the ﬁrst, last, and middle letters: def first(word):

return word[0]

def last(word):

return word[-1]

def middle(word):

return word[1:-1]

We’ll see how they work in Chapter 8.