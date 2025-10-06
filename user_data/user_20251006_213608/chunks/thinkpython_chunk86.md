>>> principal = 327.68 >>> interest = principle * rate NameError: name

’

’

principle

is not defined

Variables names are case sensitive, so LaTeX is not the same as latex.

At this point the most likely cause of a semantic error is the order of operations. For exam- ple, to evaluate 1 >>> 1.0 / 2.0 * pi

2π, you might be tempted to write

But the division happens ﬁrst, so you would get π/2, which is not the same thing! There is no way for Python to know what you meant to write, so in this case you don’t get an error message; you just get the wrong answer.

2.11 Glossary

value: One of the basic units of data, like a number or string, that a program manipulates.

type: A category of values. The types we have seen so far are integers (type int), ﬂoating-

point numbers (type float), and strings (type str).

integer: A type that represents whole numbers.

ﬂoating-point: A type that represents numbers with fractional parts.

string: A type that represents sequences of characters.