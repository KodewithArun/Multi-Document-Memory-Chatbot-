Suppose you are writing a function that works with Hand objects. You would like it to work with all kinds of Hands, like PokerHands, BridgeHands, etc. If you invoke a method like shuffle, you might get the one deﬁned in Deck, but if any of the subclasses override this method, you’ll get that version instead.

Any time you are unsure about the ﬂow of execution through your program, the sim- If plest solution is to add print statements at the beginning of the relevant methods.

18.10. Data encapsulation

Deck.shuffle prints a message that says something like Running Deck.shuffle, then as the program runs it traces the ﬂow of execution.

As an alternative, you could use this function, which takes an object and a method name (as a string) and returns the class that provides the deﬁnition of the method:

def find_defining_class(obj, meth_name):

for ty in type(obj).mro():

if meth_name in ty.__dict__:

return ty

Here’s an example: