In each state, what events can occur? In the example, the user can press either of the buttons, or quit.

For each state-event pair, what is the desired outcome? Since there are two states and two buttons, there are four state-event pairs to consider.

What can cause a transition from one state to another? In this case, there is a transition when the user creates the ﬁrst circle.

You might also ﬁnd it useful to deﬁne, and check, invariants that should hold regardless of the sequence of events.

This approach to GUI programming can help you write correct code without taking the time to test every possible sequence of user events!

19.10 Glossary

GUI: A graphical user interface.

widget: One of the elements that makes up a GUI, including buttons, menus, text entry

ﬁelds, etc.

option: A value that controls the appearance or function of a widget.

keyword argument: An argument that indicates the parameter name as part of the func-

tion call.