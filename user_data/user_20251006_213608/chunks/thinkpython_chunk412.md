’

168

Chapter 18. Inheritance

The mapping for ranks is fairly obvious; each of the numerical ranks maps to the corre- sponding integer, and for face cards:

Jack Queen King

(cid:55)→ 11 (cid:55)→ 12 (cid:55)→ 13

I am using the (cid:55)→ symbol to make it clear that these mappings are not part of the Python program. They are part of the program design, but they don’t appear explicitly in the code.

The class deﬁnition for Card looks like this: class Card(object):

"""Represents a standard playing card."""

def __init__(self, suit=0, rank=2):

self.suit = suit self.rank = rank

As usual, the init method takes an optional parameter for each attribute. The default card is the 2 of Clubs.

To create a Card, you call Card with the suit and rank of the card you want. queen_of_diamonds = Card(1, 12)

18.2 Class attributes