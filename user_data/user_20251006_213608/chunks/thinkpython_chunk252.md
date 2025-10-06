,

a

b

’

’

’

b

,

]

’

’

c

’

]

10.13 Debugging

Careless use of lists (and other mutable objects) can lead to long hours of debugging. Here are some common pitfalls and ways to avoid them:

1. Don’t forget that most list methods modify the argument and return None. This is the opposite of the string methods, which return a new string and leave the original alone. If you are used to writing string code like this:

word = word.strip()

It is tempting to write list code like this:

t = t.sort()

# WRONG!

Because sort returns None, the next operation you perform with t is likely to fail.