1. Download http://thinkpython.com/code/Wobbler.py and run it. You should see a TurtleWorld with three Turtles. If you press the Run button, the Turtles wander at random.

2. Read the code and make sure you understand how it works. The Wobbler class inherits from Turtle, which means that the Turtle methods lt, rt, fd and bk work on Wobblers.

The step method gets invoked by TurtleWorld. It invokes steer, which turns the Turtle in the desired direction, wobble, which makes a random turn in proportion to the Turtle’s clumsiness, and move, which moves forward a few pixels, depending on the Turtle’s speed.

3. Create a ﬁle named Tagger.py. Import everything from Wobbler, then deﬁne a class named Tagger that inherits from Wobbler. Call make_world passing the Tagger class object as an argument.