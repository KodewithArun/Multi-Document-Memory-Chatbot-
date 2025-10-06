As an example, we’ll write a function that takes two points, the center of the circle and a point on the perimeter, and computes the area of the circle.

Assume that the center point is stored in the variables xc and yc, and the perimeter point is in xp and yp. The ﬁrst step is to ﬁnd the radius of the circle, which is the distance between the two points. We just wrote a function, distance, that does that:

radius = distance(xc, yc, xp, yp)

The next step is to ﬁnd the area of a circle with that radius; we just wrote that, too:

result = area(radius)

Encapsulating these steps in a function, we get:

def circle_area(xc, yc, xp, yp):

radius = distance(xc, yc, xp, yp) result = area(radius) return result

The temporary variables radius and result are useful for development and debugging, but once the program is working, we can make it more concise by composing the function calls:

def circle_area(xc, yc, xp, yp):

return area(distance(xc, yc, xp, yp))

6.4 Boolean functions