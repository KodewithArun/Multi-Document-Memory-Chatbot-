Since we invoke join on a newline character, the cards are separated by newlines. Here’s what the result looks like:

>>> deck = Deck() >>> print deck Ace of Clubs 2 of Clubs 3 of Clubs ... 10 of Spades Jack of Spades Queen of Spades King of Spades

Even though the result appears on 52 lines, it is one long string that contains newlines.

18.6 Add, remove, shufﬂe and sort

To deal cards, we would like a method that removes a card from the deck and returns it. The list method pop provides a convenient way to do that:

#inside class Deck:

def pop_card(self):

return self.cards.pop()

Since pop removes the last card in the list, we are dealing from the bottom of the deck. In real life “bottom dealing” is frowned upon, but in this context it’s ok.

To add a card, we can use the list method append:

#inside class Deck:

def add_card(self, card):

self.cards.append(card)