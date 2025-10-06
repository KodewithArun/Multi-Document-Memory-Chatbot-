19.9 Debugging

One of the challenges of GUI programming is keeping track of which things happen while the GUI is being built and which things happen later in response to user events.

For example, when you are setting up a callback, it is a common error to call the function rather than passing a reference to it:

def the_callback(): ’

’

print

Called.

g.bu(text=

’

This is wrong!

’

, command=the_callback())

If you run this code, you will see that it calls the_callback immediately, and then creates the button. When you press the button, it does nothing because the return value from the_callback is None. Usually you do not want to invoke a callback while you are setting up the GUI; it should only be invoked later in response to a user event.