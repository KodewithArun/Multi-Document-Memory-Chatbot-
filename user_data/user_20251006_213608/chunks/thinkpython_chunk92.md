>>> radians = 0.7 >>> height = math.sin(radians)

The ﬁrst example uses log10 to compute a signal-to-noise ratio in decibels (assuming that signal_power and noise_power are deﬁned). The math module also provides log, which computes logarithms base e.

The second example ﬁnds the sine of radians. The name of the variable is a hint that sin and the other trigonometric functions (cos, tan, etc.) take arguments in radians. To convert from degrees to radians, divide by 360 and multiply by 2π:

>>> degrees = 45 >>> radians = degrees / 360.0 * 2 * math.pi >>> math.sin(radians) 0.707106781187

The expression math.pi gets the variable pi from the math module. The value of this variable is an approximation of π, accurate to about 15 digits.

If you know your trigonometry, you can check the previous result by comparing it to the square root of two divided by two:

>>> math.sqrt(2) / 2.0 0.707106781187

3.4. Composition

3.4 Composition