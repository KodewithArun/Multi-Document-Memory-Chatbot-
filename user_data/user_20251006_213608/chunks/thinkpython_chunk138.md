Strictly speaking, the operands of the logical operators should be boolean expressions, but Python is not very strict. Any nonzero number is interpreted as “true.” >>> 17 and True True

This ﬂexibility can be useful, but there are some subtleties to it that might be confusing. You might want to avoid it (unless you know what you are doing).

5.4 Conditional execution

In order to write useful programs, we almost always need the ability to check conditions and change the behavior of the program accordingly. Conditional statements give us this ability. The simplest form is the if statement: if x > 0: print

’

’

x is positive

The boolean expression after if is called the condition. statement gets executed. If not, nothing happens.

If it is true, then the indented

if statements have the same structure as function deﬁnitions: a header followed by an indented body. Statements like this are called compound statements.