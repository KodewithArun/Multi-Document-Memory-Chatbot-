def make_circle(event):

pos = ca.canvas_coords([event.x, event.y]) item = ca.circle(pos, 5, fill=

’

’

red

)

19.8. Binding

The Event object contains information about the type of event and details like the coordi- nates of the mouse pointer. In this example the information we need is the location of the mouse click. These values are in “pixel coordinates,” which are deﬁned by the underlying graphical system. The method canvas_coords translates them to “Canvas coordinates,” which are compatible with Canvas methods like circle.

For Entry widgets, it is common to bind the <Return> event, which is triggered when the user presses the Return or Enter key. For example, the following code creates a Button and an Entry.

’

’

Make text item:

bu = g.bu( en = g.en() en.bind(

, make_text)

’

’

<Return>

, make_text)