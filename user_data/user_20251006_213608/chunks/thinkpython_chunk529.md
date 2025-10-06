lumpy.class_diagram()

Figure C.7 shows the result. Each class is represented with a box that contains the name of the class, any methods the class provides, any class variables, and any instance variables. In this example, Rectangle and Point have instance variables, but no methods or class variables.

The arrow from Rectangle to Point shows that Rectangles contain an embedded Point. In addition, Rectangle and Point both inherit from object, which is represented in the diagram with a triangle-headed arrow.

217

218

Appendix C. Lumpy

Here’s a more complex example using my solution to Exercise 18.6. You can download the code from http://thinkpython.com/code/lumpy_demo8.py; you will also need http: //thinkpython.com/code/PokerHand.py.

from swampy.Lumpy import Lumpy

from PokerHand import *

lumpy = Lumpy() lumpy.make_reference()

deck = Deck() hand = PokerHand() deck.move_cards(hand, 7)

lumpy.class_diagram()