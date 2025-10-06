Another challenge of GUI programming is that you don’t have control of the ﬂow of exe- cution. Which parts of the program execute and their order are determined by user actions. That means that you have to design your program to work correctly for any possible se- quence of events.

For example, the GUI in Exercise 19.3 has two widgets: one creates a Circle item and the other changes the color of the Circle. If the user creates the circle and then changes its color, there’s no problem. But what if the user changes the color of a circle that doesn’t exist yet? Or creates more than one circle?

19.10. Glossary

As the number of widgets grows, it is increasingly difﬁcult to imagine all possible se- quences of events. One way to manage this complexity is to encapsulate the state of the system in an object and then consider:

What are the possible states? In the Circle example, we might consider two states: before and after the user creates the ﬁrst circle.