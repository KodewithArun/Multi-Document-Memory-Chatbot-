’

’

w

To write a ﬁle, you have to open it with mode

as a second parameter:

’

’

’

’

,

output.txt

)

w

>>> fout = open( >>> print fout <open file

’

’

’

’

output.txt

, mode

w

at 0xb7eb2410>

If the ﬁle already exists, opening it in write mode clears out the old data and starts fresh, so be careful! If the ﬁle doesn’t exist, a new one is created.

The write method puts data into the ﬁle.

134

Chapter 14. Files

>>> line1 = "This here >>> fout.write(line1)

’

s the wattle,\n"

Again, the ﬁle object keeps track of where it is, so if you call write again, it adds the new data to the end.

>>> line2 = "the emblem of our land.\n" >>> fout.write(line2)

When you are done writing, you have to close the ﬁle.

>>> fout.close()

14.3 Format operator

The argument of write has to be a string, so if we want to put other values in a ﬁle, we have to convert them to strings. The easiest way to do that is with str:

>>> x = 52 >>> fout.write(str(x))