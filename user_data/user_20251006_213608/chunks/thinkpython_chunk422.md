This relationship between classes—similar, but different—lends itself to inheritance.

The deﬁnition of a child class is like other class deﬁnitions, but the name of the parent class appears in parentheses:

class Hand(Deck):

"""Represents a hand of playing cards."""

This deﬁnition indicates that Hand inherits from Deck; that means we can use methods like pop_card and add_card for Hands as well as Decks.

Hand also inherits __init__ from Deck, but it doesn’t really do what we want: instead of populating the hand with 52 new cards, the init method for Hands should initialize cards with an empty list.

If we provide an init method in the Hand class, it overrides the one in the Deck class:

# inside class Hand:

def __init__(self, label=

’’

):

self.cards = [] self.label = label

18.8. Class diagrams

So when you create a Hand, Python invokes this init method: ’

’

>>> hand = Hand( >>> print hand.cards [] >>> print hand.label new hand

new hand

)