bbox is a list of lists that represents the “bounding box” of the rectangle. The ﬁrst pair of coordinates is the lower-left corner of the rectangle; the second pair is the upper-right corner.

You can draw a circle like this:

149

150

Chapter 15. Classes and objects

canvas.circle([-25,0], 70, outline=None, fill=

’

red

’

)

The ﬁrst parameter is the coordinate pair for the center of the circle; the second parameter is the radius.

If you add this line to the program, the result should resemble the national ﬂag of Bangladesh (see http://en.wikipedia.org/wiki/Gallery_of_sovereign-state_flags).

1. Write a function called draw_rectangle that takes a Canvas and a Rectangle as arguments and draws a representation of the Rectangle on the Canvas.

2. Add an attribute named color to your Rectangle objects and modify draw_rectangle so that it uses the color attribute as the ﬁll color.