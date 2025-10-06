Each time through, it prompts the user with an angle bracket. If the user types done, the break statement exits the loop. Otherwise the program echoes whatever the user types and goes back to the top of the loop. Here’s a sample run:

> not done not done > done Done!

This way of writing while loops is common because you can check the condition anywhere in the loop (not just at the top) and you can express the stop condition afﬁrmatively (“stop when this happens”) rather than negatively (“keep going until that happens.”).

7.5 Square roots

Loops are often used in programs that compute numerical results by starting with an ap- proximate answer and iteratively improving it.

For example, one way of computing square roots is Newton’s method. Suppose that you want to know the square root of a. If you start with almost any estimate, x, you can com- pute a better estimate with the following formula:

y =

x + a/x 2

For example, if a is 4 and x is 3: