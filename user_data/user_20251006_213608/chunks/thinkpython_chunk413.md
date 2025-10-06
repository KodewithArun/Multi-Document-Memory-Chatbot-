18.2 Class attributes

In order to print Card objects in a way that people can easily read, we need a mapping from the integer codes to the corresponding ranks and suits. A natural way to do that is with lists of strings. We assign these lists to class attributes: # inside class Card:

’

suit_names = [ rank_names = [None, ,

Clubs

’

’

’

’

8

,

9

’ ’ ’

’

, Ace ’ 10

Diamonds ’ ’ , 2 Jack

’

,

’

’

,

’ ’

,

, 3

’ ’

’

Hearts ’ 4

’

, Queen

, ’

,

’ ’

, 5 ’

’

Spades ’ 6 ’

’

’

, King

,

]

’ ’

] 7

’

,

def __str__(self):

’

return

%s of %s

’

% (Card.rank_names[self.rank], Card.suit_names[self.suit])

Variables like suit_names and rank_names, which are deﬁned inside a class but outside of any method, are called class attributes because they are associated with the class object Card.

This term distinguishes them from variables like suit and rank, which are called instance attributes because they are associated with a particular instance.