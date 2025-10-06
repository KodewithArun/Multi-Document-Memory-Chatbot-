189

190

Chapter 19. Case study: Tkinter

19.11 Exercises

Exercise 19.4. For this exercise, you will write an image viewer. Here is a simple example:

g = Gui() canvas = g.ca(width=300) photo = PhotoImage(file= canvas.image([0,0], image=photo) g.mainloop()

’

danger.gif

’

)

PhotoImage reads a ﬁle and returns a PhotoImage object that Tkinter can display. Canvas.image puts the image on the canvas, centered on the given coordinates. You can also put images on labels, buttons, and some other widgets:

g.la(image=photo) g.bu(image=photo)

PhotoImage can only handle a few image formats, like GIF and PPM, but we can use the Python Imaging Library (PIL) to read other ﬁles.

The name of the PIL module is Image, but Tkinter deﬁnes an object with the same name. To avoid the conﬂict, you can use import...as like this:

import Image as PIL import ImageTk