Python 2 provides a built-in function called raw_input that gets input from the keyboard. In Python 3, it is called input. When this function is called, the program stops and waits for the user to type something. When the user presses Return or Enter, the program resumes and raw_input returns what the user typed as a string.

>>> text = raw_input() What are you waiting for? >>> print text What are you waiting for?

5.12. Debugging

Before getting input from the user, it is a good idea to print a prompt telling the user what to input. raw_input can take a prompt as an argument:

’

>>> name = raw_input( What...is your name? Arthur, King of the Britons! >>> print name Arthur, King of the Britons!

What...is your name?\n

’

)

The sequence \n at the end of the prompt represents a newline, which is a special character that causes a line break. That’s why the user’s input appears below the prompt.

If you expect the user to type an integer, you can try to convert the return value to int: