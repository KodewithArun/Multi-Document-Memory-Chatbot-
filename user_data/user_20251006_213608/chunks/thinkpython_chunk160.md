In this case, the inputs are two points, which you can represent using four numbers. The return value is the distance, which is a ﬂoating-point value.

Already you can write an outline of the function:

def distance(x1, y1, x2, y2):

return 0.0

Obviously, this version doesn’t compute distances; it always returns zero. But it is syn- tactically correct, and it runs, which means that you can test it before you make it more complicated.

To test the new function, call it with sample arguments:

6.2. Incremental development

>>> distance(1, 2, 4, 6) 0.0

I chose these values so that the horizontal distance is 3 and the vertical distance is 4; that way, the result is 5 (the hypotenuse of a 3-4-5 triangle). When testing a function, it is useful to know the right answer.