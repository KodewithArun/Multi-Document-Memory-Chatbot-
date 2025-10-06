# inside class Card:

def __cmp__(self, other):

t1 = self.suit, self.rank t2 = other.suit, other.rank return cmp(t1, t2)

The built-in function cmp has the same interface as the method __cmp__: it takes two values and returns a positive number if the ﬁrst is larger, a negative number if the second is larger, and 0 if they are equal.

In Python 3, cmp no longer exists, and the __cmp__ method is not supported. Instead you should provide __lt__, which returns True if self is less than other. You can implement __lt__ using tuples and the < operator. Exercise 18.1. Write a __cmp__ method for Time objects. Hint: you can use tuple comparison, but you also might consider using integer subtraction.

18.4 Decks

Now that we have Cards, the next step is to deﬁne Decks. Since a deck is made up of cards, it is natural for each Deck to contain a list of cards as an attribute.