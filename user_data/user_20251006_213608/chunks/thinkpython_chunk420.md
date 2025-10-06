#inside class Deck:

def add_card(self, card):

self.cards.append(card)

A method like this that uses another function without doing much real work is sometimes called a veneer. The metaphor comes from woodworking, where it is common to glue a thin layer of good quality wood to the surface of a cheaper piece of wood.

171

172

Chapter 18. Inheritance

In this case we are deﬁning a “thin” method that expresses a list operation in terms that are appropriate for decks.

As another example, we can write a Deck method named shuffle using the function shuffle from the random module:

# inside class Deck:

def shuffle(self):

random.shuffle(self.cards)

Don’t forget to import random. Exercise 18.2. Write a Deck method named sort that uses the list method sort to sort the cards in a Deck. sort uses the __cmp__ method we deﬁned to determine sort order.

18.7 Inheritance