index = 0 while index < len(fruit): letter = fruit[index] print letter index = index + 1

This loop traverses the string and displays each letter on a line by itself. The loop condition is index < len(fruit), so when index is equal to the length of the string, the condition is false, and the body of the loop is not executed. The last character accessed is the one with the index len(fruit)-1, which is the last character in the string. Exercise 8.1. Write a function that takes a string as an argument and displays the letters backward, one per line.

Another way to write a traversal is with a for loop:

for char in fruit: print char

Each time through the loop, the next character in the string is assigned to the variable char. The loop continues until no characters are left.