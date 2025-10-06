3.13. Importing with from

Dividing a long program into functions allows you to debug the parts one at a time and then assemble them into a working whole.

Well-designed functions are often useful for many programs. Once you write and debug one, you can reuse it.

3.13

Importing with from

Python provides two ways to import modules; we have already seen one: >>> import math >>> print math ’ <module >>> print math.pi 3.14159265359

’

math

(built-in)>

If you import math, you get a module object named math. The module object contains constants like pi and functions like sin and exp.

But if you try to access pi directly, you get an error. >>> print pi Traceback (most recent call last):

File "<stdin>", line 1, in <module> ’

’

NameError: name

pi

is not defined

As an alternative, you can import an object from a module like this: >>> from math import pi

Now you can access pi directly, without dot notation. >>> print pi 3.14159265359