What kind of error it was, and

Where it occurred.

Syntax errors are usually easy to ﬁnd, but there are a few gotchas. Whitespace errors can be tricky because spaces and tabs are invisible and we are used to ignoring them.

>>> x = 5 >>>

y = 6

File "<stdin>", line 1

y = 6 ^

IndentationError: unexpected indent

In this example, the problem is that the second line is indented by one space. But the error message points to y, which is misleading. In general, error messages indicate where the problem was discovered, but the actual error might be earlier in the code, sometimes on a previous line.

’

47

48

Chapter 5. Conditionals and recursion

The same is true of runtime errors.

Suppose you are trying to compute a signal-to-noise ratio in decibels. The formula is SNRdb = 10log10(Psignal/Pnoise). In Python, you might write something like this: import math signal_power = 9 noise_power = 10 ratio = signal_power / noise_power decibels = 10 * math.log10(ratio) print decibels