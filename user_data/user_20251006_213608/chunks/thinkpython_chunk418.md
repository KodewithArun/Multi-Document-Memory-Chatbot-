The following is a class deﬁnition for Deck. The init method creates the attribute cards and generates the standard set of ﬁfty-two cards:

class Deck(object):

def __init__(self): self.cards = [] for suit in range(4):

for rank in range(1, 14):

card = Card(suit, rank) self.cards.append(card)

The easiest way to populate the deck is with a nested loop. The outer loop enumerates the suits from 0 to 3. The inner loop enumerates the ranks from 1 to 13. Each iteration creates a new Card with the current suit and rank, and appends it to self.cards.

18.5. Printing the deck

18.5 Printing the deck

Here is a __str__ method for Deck:

#inside class Deck:

def __str__(self):

res = [] for card in self.cards:

res.append(str(card))

’

’

return

\n

.join(res)

This method demonstrates an efﬁcient way to accumulate a large string: building a list of strings and then using join. The built-in function str invokes the __str__ method on each card and returns the string representation.