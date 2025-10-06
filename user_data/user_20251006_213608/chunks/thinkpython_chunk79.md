2.6 Interactive mode and script mode

One of the beneﬁts of working with an interpreted language is that you can test bits of code in interactive mode before you put them in a script. But there are differences between interactive mode and script mode that can be confusing.

For example, if you are using Python as a calculator, you might type

>>> miles = 26.2 >>> miles * 1.61 42.182

The ﬁrst line assigns a value to miles, but it has no visible effect. The second line is an ex- pression, so the interpreter evaluates it and displays the result. So we learn that a marathon is about 42 kilometers.

But if you type the same code into a script and run it, you get no output at all. In script mode an expression, all by itself, has no visible effect. Python actually evaluates the ex- pression, but it doesn’t display the value unless you tell it to:

miles = 26.2 print miles * 1.61

This behavior can be confusing at ﬁrst.