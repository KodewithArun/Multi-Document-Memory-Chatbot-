for ty in type(obj).mro():

if meth_name in ty.__dict__:

return ty

Here’s an example:

>>> hand = Hand() >>> print find_defining_class(hand, ’ <class

’

Card.Deck

>

’

shuffle

’

)

So the shuffle method for this Hand is the one in Deck.

find_defining_class uses the mro method to get the list of class objects (types) that will be searched for methods. “MRO” stands for “method resolution order.”

Here’s a program design suggestion: whenever you override a method, the interface of the new method should be the same as the old. It should take the same parameters, return the same type, and obey the same preconditions and postconditions. If you obey this rule, you will ﬁnd that any function designed to work with an instance of a superclass, like a Deck, will also work with instances of subclasses like a Hand or PokerHand.

If you violate this rule, your code will collapse like (sorry) a house of cards.

18.10 Data encapsulation