3. Write a function called draw_point that takes a Canvas and a Point as arguments and draws a representation of the Point on the Canvas.

4. Deﬁne a new class called Circle with appropriate attributes and instantiate a few Circle ob- jects. Write a function called draw_circle that draws circles on the canvas.

5. Write a program that draws the national ﬂag of the Czech Republic. Hint: you can draw a polygon like this:

points = [[-150,-100], [150, 100], [150, -100]] canvas.polygon(points, fill=

’

’

blue

)

I have written a small program that lists the available colors; you can download it from http: //thinkpython.com/code/color_list.py.

Chapter 16

Classes and functions

Code examples from this chapter are available from http://thinkpython.com/code/ Time1.py.

16.1 Time

As another example of a user-deﬁned type, we’ll deﬁne a class called Time that records the time of day. The class deﬁnition looks like this: class Time(object):

"""Represents the time of day.