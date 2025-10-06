Scale down the input: If possible, reduce the size of the dataset. For example if the pro- gram reads a text ﬁle, start with just the ﬁrst 10 lines, or with the smallest example you can ﬁnd. You can either edit the ﬁles themselves, or (better) modify the program so it reads only the ﬁrst n lines.

If there is an error, you can reduce n to the smallest value that manifests the error, and then increase it gradually as you ﬁnd and correct errors.

109

110

Chapter 11. Dictionaries

Check summaries and types: Instead of printing and checking the entire dataset, consider printing summaries of the data: for example, the number of items in a dictionary or the total of a list of numbers.

A common cause of runtime errors is a value that is not the right type. For debugging this kind of error, it is often enough to print the type of a value.