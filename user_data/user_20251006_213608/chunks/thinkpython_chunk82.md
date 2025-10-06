I don’t work very hard to remember rules of precedence for other operators. If I can’t tell by looking at the expression, I use parentheses to make it obvious.

2.8 String operations

In general, you can’t perform mathematical operations on strings, even if the strings look like numbers, so the following are illegal: ’ ’ ’

’

’

’

’

’

’

’

’

’

1



easy

/

2

eggs



third

a charm

15

16

Chapter 2. Variables, expressions and statements

The + operator works with strings, but it might not do what you expect: it performs con- catenation, which means joining the strings by linking them end-to-end. For example: first = second = print first + second The output of this program is throatwarbler.

’

’

throat ’

’

warbler

The * operator also works on strings; it performs repetition. For example, ’ SpamSpamSpam

’

. If one of the operands is a string, the other has to be an integer.

’

Spam

’