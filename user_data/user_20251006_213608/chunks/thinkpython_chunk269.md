104

Chapter 11. Dictionaries

def print_hist(h): for c in h:

print c, h[c]

Here’s what the output looks like:

>>> h = histogram( >>> print_hist(h) a 1 p 1 r 2 t 1 o 1

’

parrot

’

)

Again, the keys are in no particular order. Exercise 11.3. Dictionaries have a method called keys that returns the keys of the dictionary, in no particular order, as a list.

Modify print_hist to print the keys and their values in alphabetical order.

11.3 Reverse lookup

Given a dictionary d and a key k, it is easy to ﬁnd the corresponding value v = d[k]. This operation is called a lookup.

But what if you have v and you want to ﬁnd k? You have two problems: ﬁrst, there might be more than one key that maps to the value v. Depending on the application, you might be able to pick one, or you might have to make a list that contains all of them. Second, there is no simple syntax to do a reverse lookup; you have to search.