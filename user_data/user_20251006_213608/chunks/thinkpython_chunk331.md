One ﬁnal thought: in this discussion, I have implied that we should use one data structure for both analysis and generation. But since these are separate phases, it would also be pos- sible to use one structure for analysis and then convert to another structure for generation. This would be a net win if the time saved during generation exceeded the time spent in conversion.

13.10. Debugging

13.10 Debugging

When you are debugging a program, and especially if you are working on a hard bug, there are four things to try:

reading: Examine your code, read it back to yourself, and check that it says what you

meant to say.

running: Experiment by making changes and running different versions. Often if you dis- play the right thing at the right place in the program, the problem becomes obvious, but sometimes you have to spend some time to build scaffolding.