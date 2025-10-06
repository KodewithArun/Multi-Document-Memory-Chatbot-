Other programs are persistent: they run for a long time (or all the time); they keep at least some of their data in permanent storage (a hard drive, for example); and if they shut down and restart, they pick up where they left off.

Examples of persistent programs are operating systems, which run pretty much whenever a computer is on, and web servers, which run all the time, waiting for requests to come in on the network.

One of the simplest ways for programs to maintain their data is by reading and writing text ﬁles. We have already seen programs that read text ﬁles; in this chapter we will see programs that write them.

An alternative is to store the state of the program in a database. In this chapter I will present a simple database and a module, pickle, that makes it easy to store program data.

14.2 Reading and writing

A text ﬁle is a sequence of characters stored on a permanent medium like a hard drive, ﬂash memory, or CD-ROM. We saw how to open and read a ﬁle in Section 9.1.