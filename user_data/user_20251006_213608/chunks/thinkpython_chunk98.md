3.7. Flow of execution

As you might expect, you have to create a function before you can execute it. In other words, the function deﬁnition has to be executed before the ﬁrst time it is called. Exercise 3.1. Move the last line of this program to the top, so the function call appears before the deﬁnitions. Run the program and see what error message you get. Exercise 3.2. Move the function call back to the bottom and move the deﬁnition of print_lyrics after the deﬁnition of repeat_lyrics. What happens when you run this program?

3.7 Flow of execution

In order to ensure that a function is deﬁned before its ﬁrst use, you have to know the order in which statements are executed, which is called the ﬂow of execution.

Execution always begins at the ﬁrst statement of the program. Statements are executed one at a time, in order from top to bottom.