Figure 18.2: Class diagram.

There are several kinds of relationship between classes:

Objects in one class might contain references to objects in another class. For example, each Rectangle contains a reference to a Point, and each Deck contains references to many Cards. This kind of relationship is called HAS-A, as in, “a Rectangle has a Point.”

One class might inherit from another. This relationship is called IS-A, as in, “a Hand is a kind of a Deck.”

One class might depend on another in the sense that changes in one class would require changes in the other.

A class diagram is a graphical representation of these relationships. For example, Fig- ure 18.2 shows the relationships between Card, Deck and Hand.

The arrow with a hollow triangle head represents an IS-A relationship; in this case it indi- cates that Hand inherits from Deck.

The standard arrow head represents a HAS-A relationship; in this case a Deck has refer- ences to Card objects.