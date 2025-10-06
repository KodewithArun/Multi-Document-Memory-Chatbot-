You can see my solution at http://thinkpython.com/code/color_space.py.

Chapter 18

Inheritance

In this chapter I present classes to represent playing cards, decks of cards, and poker hands. If you don’t play poker, you can read about it at http://en.wikipedia.org/wiki/Poker, but you don’t have to; I’ll tell you what you need to know for the exercises. Code examples from this chapter are available from http://thinkpython.com/code/Card.py.

If you are not familiar with Anglo-American playing cards, you can read about them at http://en.wikipedia.org/wiki/Playing_cards.

18.1 Card objects

There are ﬁfty-two cards in a deck, each of which belongs to one of four suits and one of thirteen ranks. The suits are Spades, Hearts, Diamonds, and Clubs (in descending order in bridge). The ranks are Ace, 2, 3, 4, 5, 6, 7, 8, 9, 10, Jack, Queen, and King. Depending on the game that you are playing, an Ace may be higher than King or lower than 2.