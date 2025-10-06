35

36

Chapter 4. Case study: interface design

Rather than clutter up the interface, it is better to choose an appropriate value of n depend- ing on circumference:

def circle(t, r):

circumference = 2 * math.pi * r n = int(circumference / 3) + 1 length = circumference / n polygon(t, n, length)

Now the number of segments is (approximately) circumference/3, so the length of each segment is (approximately) 3, which is small enough that the circles look good, but big enough to be efﬁcient, and appropriate for any size circle.

4.7 Refactoring

When I wrote circle, I was able to re-use polygon because a many-sided polygon is a good approximation of a circle. But arc is not as cooperative; we can’t use polygon or circle to draw an arc.

One alternative is to start with a copy of polygon and transform it into arc. The result might look like this:

def arc(t, r, angle):