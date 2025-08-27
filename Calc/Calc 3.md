# Calc 3

## Contents

[Definitions](#Definitions)<br>


### Definitions

### Partial Differentiation

Differentiate a fn of more than one variable<br>
standard derivative: $\dfrac{df}{dx} = \lim_{h \to 0}(\dfrac{f(x+h) - f(x)}{h})$<br>
<img src="Images/limit.svg" width="420"><br>
With this, can only see the how f(x) is changing<br>
With several variables:<br>
$z=f(x,y)$ gives a surface. Gradient changes in both x and y direction<br>
$z = xy^2 + yx^3$<br>
<img src="Images/surface.png" width="420"><br>
Partial differentiation allows us to calculate rate of change for a given direction<br>
$\pdv{f}{x} = \lim+{h \to 0}(\dfrac{f(x+h, y) - f(x, y)}{h})$<br>
$\pdv{f}{y} = \lim+{h \to 0}(\dfrac{f(x, y+h) - f(x, y)}{h})$<br>

**Example 1**

$f(x,y) = xy^2 + yx^3$<br>
$\pdv{f}{x} = y^2 + 3yx^2$<br>
$\pdv{f}{y} = 2xy + x^3$

**Example 2**

$f(x,y) = (x^2 + 2x)sin(x^2+y) + e^{y-2x}$
$\pdv{f}{x} = (x^2 + 2x)cos(x^2 + y)2x + (2x + 2)sin(x^2 + y) - 2e^{y-2x}$<br>
$\pdv{f}{y} = (x^2 + 2x)cos(x^2 + y) + e^{y-2x}$