Both kinds of attribute are accessed using dot notation. For example, in __str__, self is a Card object, and self.rank is its rank. Similarly, Card is a class object, and Card.rank_names is a list of strings associated with the class.

Every card has its own suit and rank, but there is only one copy of suit_names and rank_names.

18.3. Comparing cards

listsuit_nameslistrank_namesCardtype111suitrankcard1Card

Figure 18.1: Object diagram.

Putting it all together, the expression Card.rank_names[self.rank] means “use the at- tribute rank from the object self as an index into the list rank_names from the class Card, and select the appropriate string.”

The ﬁrst element of rank_names is None because there is no card with rank zero. By includ- ing None as a place-keeper, we get a mapping with the nice property that the index 2 maps , and so on. To avoid this tweak, we could have used a dictionary instead to the string of a list.

’

’

2