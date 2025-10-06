The fill option speciﬁes that the circle should be ﬁlled in with red.

The return value from circle is an Item object that provides methods for modifying the item on the canvas. For example, you can use config to change any of the circle’s options:

181

182

Chapter 19. Case study: Tkinter

item.config(fill=

’

yellow

’

, outline=

’

orange

’

, width=10)

width is the thickness of the outline in pixels; outline is the color. Exercise 19.2. Write a program that creates a Canvas and a Button. When the user presses the Button, it should draw a circle on the canvas.

19.4 Coordinate sequences

The rectangle method takes a sequence of coordinates that specify opposite corners of the rectangle. This example draws a blue rectangle with the lower left corner at the origin and the upper right corner at (200,100):

canvas.rectangle([[0, 0], [200, 100]], , outline= fill=

’

’

blue

’

orange

’

, width=10)