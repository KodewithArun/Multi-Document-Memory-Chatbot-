5242

5205 4897

4295

3191 3130

2529

2483 2400 2364

13.5 Optional parameters

We have seen built-in functions and methods that take a variable number of arguments. It is possible to write user-deﬁned functions with optional arguments, too. For example, here is a function that prints the most common words in a histogram

def print_most_common(hist, num=10):

t = most_common(hist) print for freq, word in t[:num]: , freq

’

The most common words are:

’

’

print word,

\t

’

The ﬁrst parameter is required; the second is optional. The default value of num is 10.

If you only provide one argument:

13.6. Dictionary subtraction

print_most_common(hist) num gets the default value. If you provide two arguments: print_most_common(hist, 20) num gets the value of the argument instead. In other words, the optional argument over- rides the default value.

If a function has both required and optional parameters, all the required parameters have to come ﬁrst, followed by the optional ones.