The hard question is whether we can prove that this program terminates for all posi- tive values of n. So far, no one has been able to prove it or disprove it! (See http: //en.wikipedia.org/wiki/Collatz_conjecture.) Exercise 7.1. Rewrite the function print_n from Section 5.8 using iteration instead of recursion.

7.4 break

Sometimes you don’t know it’s time to end a loop until you get half way through the body. In that case you can use the break statement to jump out of the loop.

For example, suppose you want to take input from the user until they type done. You could write:

65

66

Chapter 7. Iteration

while True:

line = raw_input( ’ if line ==

’

done

’

:

>

’

)

break

print line

print

’

Done!

’

The loop condition is True, which is always true, so the loop runs until it hits the break statement.