def arc(t, r, angle):

arc_length = 2 * math.pi * r * angle / 360 n = int(arc_length / 3) + 1 step_length = arc_length / n step_angle = float(angle) / n

for i in range(n):

fd(t, step_length) lt(t, step_angle)

The second half of this function looks like polygon, but we can’t re-use polygon without changing the interface. We could generalize polygon to take an angle as a third argument, but then polygon would no longer be an appropriate name! Instead, let’s call the more general function polyline:

def polyline(t, n, length, angle):

for i in range(n):

fd(t, length) lt(t, angle)

Now we can rewrite polygon and arc to use polyline:

def polygon(t, n, length): angle = 360.0 / n polyline(t, n, length, angle)

def arc(t, r, angle):

arc_length = 2 * math.pi * r * angle / 360 n = int(arc_length / 3) + 1 step_length = arc_length / n step_angle = float(angle) / n polyline(t, n, step_length, step_angle)

4.8. A development plan

Finally, we can rewrite circle to use arc:

def circle(t, r):