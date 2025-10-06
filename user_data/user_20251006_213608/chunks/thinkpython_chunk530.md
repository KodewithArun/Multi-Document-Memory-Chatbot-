deck = Deck() hand = PokerHand() deck.move_cards(hand, 7)

lumpy.class_diagram()

Figure C.8 shows the result. PokerHand inherits from Hand, which inherits from Deck. Both Deck and PokerHand have Cards.

This diagram does not show that Hand also has cards, because in the program there are no instances of Hand. This example demonstrates a limitation of Lumpy; it only knows about the attributes and HAS-A relationships of objects that are instantiated.