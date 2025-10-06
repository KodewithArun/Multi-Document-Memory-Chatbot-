Programs that will be imported as modules often use the following idiom:

’

’

__main__ ’

if __name__ ==

: wc.py

print linecount(

’

)

__name__ is a built-in variable that is set when the program starts. If the program is run- ning as a script, __name__ has the value __main__; in that case, the test code is executed. Otherwise, if the module is being imported, the test code is skipped. Exercise 14.5. Type this example into a ﬁle named wc.py and run it as a script. Then run the Python interpreter and import wc. What is the value of __name__ when the module is being imported?

Warning: If you import a module that has already been imported, Python does nothing. It does not re-read the ﬁle, even if it has changed.

If you want to reload a module, you can use the built-in function reload, but it can be tricky, so the safest thing to do is restart the interpreter and then import the module again.

14.10 Debugging