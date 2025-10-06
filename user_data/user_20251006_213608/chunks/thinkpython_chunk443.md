The option that controls the behavior of a button is command. The value of command is a function that gets executed when the button is pressed. For example, here is a function that creates a new Label:

def make_label(): g.la(text=

’

Thank you.

’

)

Now we can create a button with this function as its command:

19.3. Canvas widgets

’

’

button2 = g.bu(text= When you press this button, it should execute make_label and a new label should appear.

No, press me!

, command=make_label)

The value of the command option is a function object, which is known as a callback because after you call bu to create the button, the ﬂow of execution “calls back” when the user presses the button.

This kind of ﬂow is characteristic of event-driven programming. User actions, like but- ton presses and key strokes, are called events. In event-driven programming, the ﬂow of execution is determined by user actions rather than by the programmer.