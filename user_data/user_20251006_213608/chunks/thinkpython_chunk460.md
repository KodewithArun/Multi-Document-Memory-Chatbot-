’ ’ ’

’

<Button-3> <B3-Motion> <Release-3>

, self.select) ’ , self.drag) ’ , self.drop)

The init method takes an Item as a parameter. It copies the attributes of the Item and then creates bindings for three events: a button press, button motion, and button release.

The event handler select stores the coordinates of the current event and the original color of the item, then changes the color to yellow:

def select(self, event): self.dragx = event.x self.dragy = event.y

’

self.fill = self.cget( self.config(fill=

fill ’ )

’

yellow

’

)

cget stands for “get conﬁguration;” it takes the name of an option as a string and returns the current value of that option.

drag computes how far the object has moved relative to the starting place, updates the stored coordinates, and then moves the item.

def drag(self, event):

dx = event.x - self.dragx

187

188

Chapter 19. Case study: Tkinter

dy = event.y - self.dragy

self.dragx = event.x self.dragy = event.y

self.move(dx, dy)