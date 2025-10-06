1. Download the following ﬁles from http://thinkpython.com/code:

Card.py : A complete version of the Card, Deck and Hand classes in this chapter.

PokerHand.py : An incomplete implementation of a class that represents a poker hand, and

some code that tests it.

2. If you run PokerHand.py, it deals seven 7-card poker hands and checks to see if any of them contains a ﬂush. Read this code carefully before you go on.

3. Add methods to PokerHand.py named has_pair, has_twopair, etc. that return True or False according to whether or not the hand meets the relevant criteria. Your code should work correctly for “hands” that contain any number of cards (although 5 and 7 are the most common sizes).

4. Write a method named classify that ﬁgures out the highest-value classiﬁcation for a hand and sets the label attribute accordingly. For example, a 7-card hand might contain a ﬂush and a pair; it should be labeled “ﬂush”.

177

178

Chapter 18. Inheritance