banana

’

’

:

count = count + 1

print count

This program demonstrates another pattern of computation called a counter. The variable count is initialized to 0 and then incremented each time an a is found. When the loop exits, count contains the result—the total number of a’s. Exercise 8.5. Encapsulate this code in a function named count, and generalize it so that it accepts the string and the letter as arguments. Exercise 8.6. Rewrite this function so that instead of traversing the string, it uses the three- parameter version of find from the previous section.

8.8 String methods

A method is similar to a function—it takes arguments and returns a value—but the syntax is different. For example, the method upper takes a string and returns a new string with all uppercase letters:

Instead of the function syntax upper(word), it uses the method syntax word.upper().

’

’

>>> word = >>> new_word = word.upper() >>> print new_word BANANA

banana