Card__cmp____init____str__rank_namessuit_namesranksuit

Hand__init__

Figure C.8: Class diagram.

Class diagrams are different. They show the classes that make up a program and the re- lationships between them. They are timeless in the sense that they describe the program as a whole, not any particular point in time. For example, if an instance of Class A gener- ally contains a reference to an instance of Class B, we say there is a “HAS-A relationship” between those classes.

Here’s an example that shows a HAS-A relationship. You can download it from http: //thinkpython.com/code/lumpy_demo7.py. from swampy.Lumpy import Lumpy

lumpy = Lumpy() lumpy.make_reference()

box = Rectangle() box.width = 100.0 box.height = 200.0 box.corner = Point() box.corner.x = 0.0 box.corner.y = 0.0

lumpy.class_diagram()