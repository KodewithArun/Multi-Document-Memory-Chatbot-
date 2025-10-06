The correct ordering for cards is not obvious. For example, which is better, the 3 of Clubs or the 2 of Diamonds? One has a higher rank, but the other has a higher suit. In order to compare cards, you have to decide whether rank or suit is more important.

The answer might depend on what game you are playing, but to keep things simple, we’ll make the arbitrary choice that suit is more important, so all of the Spades outrank all of the Diamonds, and so on.

With that decided, we can write __cmp__:

169

170

Chapter 18. Inheritance

# inside class Card:

def __cmp__(self, other): # check the suits if self.suit > other.suit: return 1 if self.suit < other.suit: return -1

# suits are the same... check ranks if self.rank > other.rank: return 1 if self.rank < other.rank: return -1

# ranks are the same... it return 0

’

s a tie

You can write this more concisely using tuple comparison:

# inside class Card:

def __cmp__(self, other):