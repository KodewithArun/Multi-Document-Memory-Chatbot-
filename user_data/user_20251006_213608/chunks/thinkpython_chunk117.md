wait_for_user tells TurtleWorld to wait for the user to do something, although in this case there’s not much for the user to do except close the window.

TurtleWorld provides several turtle-steering functions: fd and bk for forward and back- ward, and lt and rt for left and right turns. Also, each Turtle is holding a pen, which is either down or up; if the pen is down, the Turtle leaves a trail when it moves. The functions pu and pd stand for “pen up” and “pen down.”

To draw a right angle, add these lines to the program (after creating bob and before calling wait_for_user):

fd(bob, 100) lt(bob) fd(bob, 100)

The ﬁrst line tells bob to take 100 steps forward. The second line tells him to turn left.

When you run this program, you should see bob move east and then north, leaving two line segments behind.

Now modify the program to draw a square. Don’t go on until you’ve got it working!

4.2 Simple repetition