’

’

m a lumberjack, and I

m okay.

’

’

m a lumberjack, and I

m okay.

But that’s not really how the song goes.

3.6 Deﬁnitions and uses

Pulling together the code fragments from the previous section, the whole program looks like this: def print_lyrics():

’

’

print "I print "I sleep all night and I work all day."

m a lumberjack, and I

m okay."

def repeat_lyrics():

print_lyrics() print_lyrics()

repeat_lyrics()

This program contains two function deﬁnitions: print_lyrics and repeat_lyrics. Func- tion deﬁnitions get executed just like other statements, but the effect is to create function objects. The statements inside the function do not get executed until the function is called, and the function deﬁnition generates no output.

3.7. Flow of execution