’

’

>>> word = >>> new_word = word.upper() >>> print new_word BANANA

banana

This form of dot notation speciﬁes the name of the method, upper, and the name of the string to apply the method to, word. The empty parentheses indicate that this method takes no argument.

A method call is called an invocation; in this case, we would say that we are invoking upper on the word.

As it turns out, there is a string method named find that is remarkably similar to the function we wrote:

’

’

>>> word = >>> index = word.find( >>> print index 1

banana

’

a

’

)

In this example, we invoke find on word and pass the letter we are looking for as a param- eter.

Actually, the find method is more general than our function; it can ﬁnd substrings, not just characters:

>>> word.find( 2

’

na

’

)

75

76

Chapter 8. Strings

It can take as a second argument the index where it should start:

>>> word.find( 4

’

na

’

, 3)

And as a third argument the index where it should stop:

’

’