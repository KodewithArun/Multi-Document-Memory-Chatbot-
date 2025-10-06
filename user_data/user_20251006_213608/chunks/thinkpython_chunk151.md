But when you run it in Python 2, you get an error message.

Traceback (most recent call last):

File "snr.py", line 5, in ?

decibels = 10 * math.log10(ratio)

ValueError: math domain error

The error message indicates line 5, but there is nothing wrong with that line. To ﬁnd the real error, it might be useful to print the value of ratio, which turns out to be 0. The problem is in line 4, because dividing two integers does ﬂoor division. The solution is to represent signal power and noise power with ﬂoating-point values.

In general, error messages tell you where the problem was discovered, but that is often not where it was caused.

In Python 3, this example does not cause an error; the division operator performs ﬂoating- point division even with integer operands.

5.13 Glossary

modulus operator: An operator, denoted with a percent sign (%), that works on integers

and yields the remainder when one number is divided by another.