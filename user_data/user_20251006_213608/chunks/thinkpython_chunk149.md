If you expect the user to type an integer, you can try to convert the return value to int:

’

>>> prompt = >>> speed = raw_input(prompt) What...is the airspeed velocity of an unladen swallow? 17 >>> int(speed) 17

What...is the airspeed velocity of an unladen swallow?\n

But if the user types something other than a string of digits, you get an error:

>>> speed = raw_input(prompt) What...is the airspeed velocity of an unladen swallow? What do you mean, an African or a European swallow? >>> int(speed) ValueError: invalid literal for int() with base 10

We will see how to handle this kind of error later.

5.12 Debugging

The traceback Python displays when an error occurs contains a lot of information, but it can be overwhelming, especially when there are many frames on the stack. The most useful parts are usually:

What kind of error it was, and

Where it occurred.