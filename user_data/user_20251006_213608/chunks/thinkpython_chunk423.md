’

>>> hand = Hand( >>> print hand.cards [] >>> print hand.label new hand

new hand

)

But the other methods are inherited from Deck, so we can use pop_card and add_card to deal a card:

>>> deck = Deck() >>> card = deck.pop_card() >>> hand.add_card(card) >>> print hand King of Spades

A natural next step is to encapsulate this code in a method called move_cards: #inside class Deck:

def move_cards(self, hand, num):

for i in range(num):

hand.add_card(self.pop_card())

move_cards takes two arguments, a Hand object and the number of cards to deal. It modi- ﬁes both self and hand, and returns None.