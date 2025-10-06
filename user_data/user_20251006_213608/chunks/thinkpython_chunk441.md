This Gui doesn’t do much because it doesn’t have any widgets. Widgets are the elements that make up a GUI; they include:

Button: A widget, containing text or an image, that performs an action when pressed.

Canvas: A region that can display lines, rectangles, circles and other shapes.

Entry: A region where users can type text.

Scrollbar: A widget that controls the visible part of another widget.

Frame: A container, often invisible, that contains other widgets.

The empty gray square you see when you create a Gui is a Frame. When you create a new widget, it is added to this Frame.

19.2 Buttons and callbacks

The method bu creates a Button widget:

button = g.bu(text=

’

Press me.

’

)

The return value from bu is a Button object. The button that appears in the Frame is a graphical representation of this object; you can control the button by invoking methods on it.