14.8 Pipes

Most operating systems provide a command-line interface, also known as a shell. Shells usually provide commands to navigate the ﬁle system and launch applications. For exam- ple, in Unix you can change directories with cd, display the contents of a directory with ls, and launch a web browser by typing (for example) firefox.

Any program that you can launch from the shell can also be launched from Python using a pipe. A pipe is an object that represents a running program.

For example, the Unix command ls -l normally displays the contents of the current di- rectory (in long format). You can launch ls with os.popen1: >>> cmd = >>> fp = os.popen(cmd)

’

’

ls -l

The argument is a string that contains a shell command. The return value is an object that behaves just like an open ﬁle. You can read the output from the ls process one line at a time with readline or get the whole thing at once with read: