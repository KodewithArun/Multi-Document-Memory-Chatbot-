bu takes up to 32 parameters that control the appearance and function of the button. These parameters are called options. Instead of providing values for all 32 options, you can use ’ keyword arguments, like text= , to specify only the options you need and use the default values for the rest.

’

Press me.

When you add a widget to the Frame, it gets “shrink-wrapped;” that is, the Frame shrinks to the size of the Button. If you add more widgets, the Frame grows to accommodate them.

The method la creates a Label widget:

label = g.la(text=

’

Press the button.

’

)

By default, Tkinter stacks the widgets top-to-bottom and centers them. We’ll see how to override that behavior soon.

If you press the button, you will see that it doesn’t do much. That’s because you haven’t “wired it up;” that is, you haven’t told it what to do!