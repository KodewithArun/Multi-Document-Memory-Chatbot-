The Callable object stores a reference to the function and the arguments as attributes. Later, when the user clicks on a menu item, the callback calls the function and passes the stored arguments.

Here is what set_color might look like:

def set_color(color):

mb.config(text=color) print color

When the user selects a menu item and set_color is called, it conﬁgures the Menubutton to display the newly-selected color. It also print the color; if you try this example, you can conﬁrm that set_color is called when you select an item (and not called when you create the Callable object).

19.8 Binding

A binding is an association between a widget, an event and a callback: when an event (like a button press) happens on a widget, the callback is invoked.