This diagram might clarify two points of common confusion: (1) the difference between the class object, Point, and the instance of Point, obj, and (2) the difference between the func- tion object created when instantiate is deﬁned, and the frame created with it is called.

C.5 Class Diagrams

Although I distinguish between state diagrams, stack diagrams and object diagrams, they are mostly the same thing: they show the state of a running program at a point in time.

C.5. Class Diagrams

PokerHandhas_flushsuit_histcardslabel

Deck__init____str__add_cardmove_cardspop_cardremove_cardshufflesortcards

object

Card__cmp____init____str__rank_namessuit_namesranksuit

Hand__init__

Figure C.8: Class diagram.