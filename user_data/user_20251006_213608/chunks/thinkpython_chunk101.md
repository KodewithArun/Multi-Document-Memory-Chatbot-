Spam

)

The same rules of composition that apply to built-in functions also apply to user-deﬁned functions, so we can use any kind of expression as an argument for print_twice: >>> print_twice( Spam Spam Spam Spam Spam Spam Spam Spam >>> print_twice(math.cos(math.pi)) -1.0 -1.0

’

’

Spam

4)

The argument is evaluated before the function is called, so in the examples the expressions ’

’

Spam

4 and math.cos(math.pi) are only evaluated once.

You can also use a variable as an argument: ’ >>> michael = Eric, the half a bee. >>> print_twice(michael) Eric, the half a bee. Eric, the half a bee.

’

The name of the variable we pass as an argument (michael) has nothing to do with the name of the parameter (bruce). It doesn’t matter what the value was called back home (in the caller); here in print_twice, we call everybody bruce.

3.9 Variables and parameters are local