import Image as PIL import ImageTk

The ﬁrst line imports Image and gives it the local name PIL. The second line imports ImageTk, which can translate a PIL image into a Tkinter PhotoImage. Here’s an example:

’

’

image = PIL.open( photo2 = ImageTk.PhotoImage(image) g.la(image=photo2)

allen.png

)

1. Download image_demo.py, danger.gif and allen.png from http://thinkpython. com/code. Run image_demo.py. You might have to install PIL and ImageTk. They are probably in your software repository, but if not you can get them from http:// pythonware.com/products/pil.

2. In image_demo.py change the name of the second PhotoImage from photo2 to photo and run the program again. You should see the second PhotoImage but not the ﬁrst.

The problem is that when you reassign photo it overwrites the reference to the ﬁrst PhotoIm- age, which then disappears. The same thing happens if you assign a PhotoImage to a local variable; it disappears when the function ends.