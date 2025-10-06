4.10 Debugging

An interface is like a contract between a function and a caller. The caller agrees to provide certain parameters and the function agrees to do certain work.

For example, polyline requires four arguments: t has to be a Turtle; n is the number of line segments, so it has to be an integer; length should be a positive number; and angle has to be a number, which is understood to be in degrees.

These requirements are called preconditions because they are supposed to be true before the function starts executing. Conversely, conditions at the end of the function are post- conditions. Postconditions include the intended effect of the function (like drawing line segments) and any side effects (like moving the Turtle or making other changes in the World).

Preconditions are the responsibility of the caller. If the caller violates a (properly docu- mented!) precondition and the function doesn’t work correctly, the bug is in the caller, not the function.

4.11 Glossary