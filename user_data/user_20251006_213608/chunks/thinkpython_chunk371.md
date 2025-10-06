Or, depending on how you installed Swampy, like this: from World import World

The following code creates a World object and calls the mainloop method, which waits for the user. world = World() world.mainloop()

A window should appear with a title bar and an empty square. We will use this window to draw Points, Rectangles and other shapes. Add the following lines before calling mainloop and run the program again. canvas = world.ca(width=500, height=500, background= bbox = [[-150,-100], [150, 100]] ’ canvas.rectangle(bbox, outline=

’

’

white

)

’

’

’

green4

, width=2, fill=

black

)

You should see a green rectangle with a black outline. The ﬁrst line creates a Canvas, which appears in the window as a white square. The Canvas object provides methods like rectangle for drawing various shapes.