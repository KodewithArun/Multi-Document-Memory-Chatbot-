The challenge of event-driven programming is to construct a set of widgets and callbacks that work correctly (or at least generate appropriate error messages) for any sequence of user actions. Exercise 19.1. Write a program that creates a GUI with a single button. When the button is pressed it should create a second button. When that button is pressed, it should create a label that says, “Nice job!”.

What happens if you press the buttons more than once? Solution: http://thinkpython.com/ code/button_demo.py

19.3 Canvas widgets

One of the most versatile widgets is the Canvas, which creates a region for drawing lines, circles and other shapes. If you did Exercise 15.4 you are already familiar with canvases.

The method ca creates a new Canvas: canvas = g.ca(width=500, height=500) width and height are the dimensions of the canvas in pixels.