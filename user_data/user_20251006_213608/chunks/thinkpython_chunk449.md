’

after the ﬁrst character of the ﬁrst line. nother

nother

’

’

>>> text.insert(1.1, The get method reads the text in the widget; it takes a start and end index as arguments. The following example returns all the text in the widget, including the newline character: >>> text.get(0.0, END) ’

)

’

Another line of text.\n The delete method removes text from the widget; the following example deletes all but the ﬁrst two characters: >>> text.delete(1.2, END) >>> text.get(0.0, END) ’

’

An\n

Exercise 19.3. Modify your solution to Exercise 19.2 by adding an Entry widget and a second button. When the user presses the second button, it should read a color name from the Entry and use it to change the ﬁll color of the circle. Use config to modify the existing circle; don’t create a new one.

Your program should handle the case where the user tries to change the color of a circle that hasn’t been created, and the case where the color name is invalid.