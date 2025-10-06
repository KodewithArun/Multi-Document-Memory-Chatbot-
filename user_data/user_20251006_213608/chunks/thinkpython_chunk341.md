In the ﬁrst example, there aren’t enough elements; in the second, the element is the wrong type.

The format operator is powerful, but it can be difﬁcult to use. You can read more about it at http://docs.python.org/2/library/stdtypes.html#string-formatting.

14.4 Filenames and paths

Files are organized into directories (also called “folders”). Every running program has a “current directory,” which is the default directory for most operations. For example, when you open a ﬁle for reading, Python looks for it in the current directory.

The os module provides functions for working with ﬁles and directories (“os” stands for “operating system”). os.getcwd returns the name of the current directory:

>>> import os >>> cwd = os.getcwd() >>> print cwd /home/dinsdale

cwd stands for “current working directory.” The result in this example is /home/dinsdale, which is the home directory of a user named dinsdale.