If we want to deﬁne a new object to represent a playing card, it is obvious what the at- tributes should be: rank and suit. It is not as obvious what type the attributes should be. One possibility is to use strings containing words like for ranks. One problem with this implementation is that it would not be easy to compare cards to see which had a higher rank or suit.

’

’

’

Spade

for suits and

Queen

An alternative is to use integers to encode the ranks and suits. In this context, “encode” means that we are going to deﬁne a mapping between numbers and suits, or between numbers and ranks. This kind of encoding is not meant to be a secret (that would be “encryption”).

For example, this table shows the suits and the corresponding integer codes:

Spades Hearts Diamonds Clubs

(cid:55)→ 3 (cid:55)→ 2 (cid:55)→ 1 (cid:55)→ 0

This code makes it easy to compare cards; because higher suits map to higher numbers, we can compare suits by comparing their codes.

’

168