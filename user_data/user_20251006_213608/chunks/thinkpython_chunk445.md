After you create a widget, you can still change the values of the options with the config method. For example, the bg option changes the background color: canvas.config(bg= The value of bg is a string that names a color. The set of legal color names is different for different implementations of Python, but all implementations provide at least: white red cyan Shapes on a Canvas are called items. For example, the Canvas method circle draws (you guessed it) a circle: item = canvas.circle([0,0], 100, fill=

’

’

white

)

black green yellow

blue magenta

’

’

red

)

The ﬁrst argument is a coordinate pair that speciﬁes the center of the circle; the second is the radius.

Gui.py provides a standard Cartesian coordinate system with the origin at the center of the Canvas and the positive y axis pointing up. This is different from some other graphics systems where the origin is in the upper left corner, with the y axis pointing down.