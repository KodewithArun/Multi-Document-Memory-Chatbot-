To avoid this problem, you have to store a reference to each PhotoImage you want to keep. You can use a global variable, or store PhotoImages in a data structure or as an attribute of an object.

This behavior can be frustrating, which is why I am warning you (and why the example image says “Danger!”).

3. Starting with this example, write a program that takes the name of a directory and loops through all the ﬁles, displaying any ﬁles that PIL recognizes as images. You can use a try statement to catch the ﬁles PIL doesn’t recognize. When the user clicks on the image, the program should display the next one.

19.11. Exercises

4. PIL provides a variety of methods for manipulating images. You can read about them at http://pythonware.com/library/pil/handbook. As a challenge, choose a few of these methods and provide a GUI for applying them to images.