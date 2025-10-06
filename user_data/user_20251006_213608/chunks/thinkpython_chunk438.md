4. Add a steer method to Tagger to override the one in Wobbler. As a starting place, write a version that always points the Turtle toward the origin. Hint: use the math function atan2 and the Turtle attributes x, y and heading.

5. Modify steer so that the Turtles stay in bounds. For debugging, you might want to use the Step button, which invokes step once on each Turtle.

6. Modify steer so that each Turtle points toward its nearest neighbor. Hint: Turtles have an attribute, world, that is a reference to the TurtleWorld they live in, and the TurtleWorld has an attribute, animals, that is a list of all Turtles in the world.