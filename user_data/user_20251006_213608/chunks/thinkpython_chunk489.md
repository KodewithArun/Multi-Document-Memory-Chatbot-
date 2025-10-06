A.3.3

I’ve got a function or method that doesn’t return what I expect.

If you have a return statement with a complex expression, you don’t have a chance to print the return value before returning. Again, you can use a temporary variable. For example, instead of: return self.hands[i].removeMatches()

you could write: count = self.hands[i].removeMatches() return count Now you have the opportunity to display the value of count before returning.

199

200

Appendix A. Debugging

A.3.4

I’m really, really stuck and I need help.

First, try getting away from the computer for a few minutes. Computers emit waves that affect the brain, causing these symptoms:

Frustration and rage.

Superstitious beliefs (“the computer hates me”) and magical thinking (“the program only works when I wear my hat backward”).

Random walk programming (the attempt to program by writing every possible pro- gram and choosing the one that does the right thing).