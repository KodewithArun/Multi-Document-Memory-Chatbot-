As a noun, “AT-trib-ute” is pronounced with emphasis on the ﬁrst syllable, as opposed to “a-TRIB-ute,” which is a verb.

The following diagram shows the result of these assignments. A state diagram that shows an object and its attributes is called an object diagram; see Figure 15.1.

The variable blank refers to a Point object, which contains two attributes. Each attribute refers to a ﬂoating-point number.

You can read the value of an attribute using the same syntax: >>> print blank.y 4.0 >>> x = blank.x >>> print x 3.0 The expression blank.x means, “Go to the object blank refers to and get the value of x.” In this case, we assign that value to a variable named x. There is no conﬂict between the variable x and the attribute x.

You can use dot notation as part of any expression. For example:

15.3. Rectangles

’

’

>>> print (3.0, 4.0) >>> distance = math.sqrt(blank.x**2 + blank.y**2) >>> print distance 5.0

(%g, %g)

% (blank.x, blank.y)