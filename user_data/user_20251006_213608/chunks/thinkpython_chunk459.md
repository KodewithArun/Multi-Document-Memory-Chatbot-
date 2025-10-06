’

’

Make text item:

bu = g.bu( en = g.en() en.bind(

, make_text)

’

’

<Return>

, make_text)

make_text is called when the Button is pressed or when the user hits Return while typing in the Entry. To make this work, we need a function that can be called as a command (with no arguments) or as an event handler (with an Event as an argument):

def make_text(event=None):

text = en.get() item = ca.text([0,0], text)

make_text gets the contents of the Entry and displays it as a Text item in the Canvas.

It is also possible to create bindings for Canvas items. The following is a class deﬁnition for Draggable, which is a child class of Item that provides bindings that implement drag- and-drop capability.

class Draggable(Item):

def __init__(self, item):

self.canvas = item.canvas self.tag = item.tag self.bind( self.bind( self.bind(

’ ’ ’

’

<Button-3> <B3-Motion> <Release-3>

, self.select) ’ , self.drag) ’ , self.drop)