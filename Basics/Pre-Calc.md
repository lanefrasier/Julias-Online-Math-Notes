# Pre-Calc

## Contents

[Important Math Notations/Definitions](#important-math-notationsdefinitions)<br>
[Functions](#functions)<br>
[Finding Domain](#finding-domain)<br>
[Properties of a function](#properties-of-a-function)<br>
[Average rate of change](#average-rate-of-change)<br>
[Popular graphs](#popular-graphs)<br>
[Transformations](#transformations)<br>
[Solving Quadratics](#solving-quadratics)<br>
[Polynomial Functions](#polynomial-functions)<br>
[Power Functions](#power-functions)<br>

### Important Math Notations/Definitions

**Inclusive set** [ ] <br>
**Exclusive set** ( ) - always used with $\infty$<br>
**Domain:** Set of inputs of a function that give a **real** number output, square roots need to be positive. Always find domain of function before operations.<br>
**Range:** Set of outputs<br>
**Codomain:** Domain of the output<br>
**Intersection:** $a \cap b$ has the elements which are common to both set a and set b.<br>
**Union:** $a \cup b$ contains all elements that are in at least one of the sets with duplicates removed. <br>

### Functions
A function is a relationship that maps **one input** ($x$ values) to **one output** ($y$ or $f(x)$ values). An input **never** gives more than 1 output.

**Even function** symmetric about the y-axis <br>
$f(x) = f(-x)$

**Odd function** Symmetric about the origin - rotate 180 and fold twice over y then x <br>
$-f(x) = f(-x)$

<img src="Images/even-odd-fn.png" width="420" alt="Even/Odd fn"><br>

> **Example 1:** two inputs share one output - still a function

| Work Hours |   | Pay |
|-----------:|:-:|----:|
| 2 hrs      | → | $30 |
| 4 hrs      | → | $60 |
| 6 hrs      | → | $90 |
| 8 hrs      | → | $90 |  

$S = \set{(-2, 16), (-1,4), (0,3)}$<br>
$y = -7x +5$<br>
$y= 2x^2 -5x +4$<br>

> **Example 2:** one input has two outputs - not a function

| Work Hours |   | Pay |
|-----------:|:-:|----:|
| 2 hrs      | → | $30 |
| 4 hrs      | → | $60 |
| 4 hrs      | → | $90 |

$R = \set{(-2, 16), (-1,4), (-2,16)}$<br>
$y = \pm\sqrt{3-2x}$

> **Example 3:** Denominators can never equal 0

$g(t) = \frac{5t}{t^3 -16t}$<br>$t^3 - 16t = 0$<br>$t(t^2 -16) = 0$<br>$t(t-4)(t+4) = 0$<br>

$D:\{\, t \mid t\in\mathbb{R}, t \neq -4, t \neq 0, t \neq 4\,\}$<br>
$(-\infty, -4) \cup (-4, 0) \cup (0, 4) \cup (4, \infty)$

> **Example 4:** Vertical line test<br>
If a vertical line passes through the graph more than once - not a function. <br>
<img src="Images/vertical_line_test_false.svg" width="220" alt="Fails V-line test"> <img src="Images/vertical_line_test_true.svg" width="220" alt="Passes V-line test">

### Finding Domain

> **Example 1:** Finding solution to equality

$f(x) = \sqrt{5-4x}$<br>$5-4x \ge 0$<br>$x \ge \frac{5}{4}$<br>

Domain = $\set{x \mid x \le \frac{5}{4}}$

### Properties of a function

**Equation of a line** $y -y_1 = m(x-x_1)$<br>
**Increasing** $x_1 < x_2$ for $f(x_1) < f(x_2)$<br>
**Decreasing** $x_1 < x_2$ for $f(x_1) > f(x_2)$<br>
<img src="Images/Increasedecrease.png" width="420"><br>

**Local/Relative Max** On an open interval $f(x) \le f(c)$ where $c$ is a local max. Function changes from increasing to decreasing. Cannot ocur at an endpoint.<br>
**Local/Relative Min** $f(x) \ge f(c)$ where $c$ is a local min. Function changes from decreasing to increasing. Cannot occur at an endpoint. <br>
**Absolute Max** Highest output of the function. Can occur at endpoints.<br>
**Absolute Min** Lowest output of the function. Can occur at endpoints.<br>
<img src="Images/abslocalmaxmin.png" width="420"><br>

### Average rate of change 

$\frac{f(b) - f(a)}{b-a}$<br>
> **Example** Find Average rate of change of $f(x) = x^2 - 2x$ from $x = 3$ to $x=5$<br>
$f(3) = 9-6 = 3$<br>
$f(5) = 25-10 = 15$<br>
Average rate of change $\frac{15 -3}{5-3} = \frac{12}{2} = 6$<br>

### Popular graphs

Piece-wise functions<br>
<img src="Images/piece-wise.png" width="420">

$f(x) = 3$ <br>
<img src="Images/constant.gif" width="420"><br>

$f(x) = x$<br>
<img src="Images/x.png" width="420"><br>

$f(x) = \sqrt[3]{x}$ and $f(x) = \sqrt[2]{x}$<br>
<img src="Images/rootx.png" width="420"><br>

$f(x) = |x|$<br>
<img src="Images/absolutevalue.jpg" width="420"><br>

$f(x) = \frac{1}{x}$<br>
<img src="Images/1overx.png" width="420"><br>

### Transformations<br>
**Vertical:** <br>
$f(x) + k$ - shift up<br>
$f(x) -k$ - shift down<br>
When $y = af(x)$:<br>
$a>1$ stretch<br>
$a<1$ compress<br>

**Horizontal:**<br>
$f(x+h)$ shift left <br>
$f(x-h)$ shift right <br>

**Reflection:**<br>
$y = -f(x)$ reflect x-axis<br>
$y = f(-x)$ reflect y-axis<br>

Odd key points (plot these to find shape)<br>
$(1, 1)$
$(0, 0)$
$(-1, -1)$

Even key points(plot these to find shape)<br>
$(1, 1)$
$(0, 0)$
$(-1, 1)$

### Quadratics

$f(x) = ax^{2} +bx +c$ --> $x = \frac{-b \pm\sqrt{b^{2} - 4ac}}{2a}$<br>
if discriminant > 0 -> 2 solutions
if discriminant = 0 -> 1 solution
if discriminant < 0 -> no real solution

> **Square Root Method**<br>
Get $x^2$ by itself - no other x's in the equation

1. $f(x) = x^{2} -18$<br>
   $x^{2} = 18$<br>
   $x = \pm\sqrt{18} = \pm\sqrt{9 \cdot 2} = \pm 3 \sqrt{2}$<br>
2. $h(x) = (2x +3)^{2} - 32$ <br>
   $(2x+3)^{2} = 32$<br>
   $(2x+3) = \pm\sqrt{32} = \pm\sqrt{2 \cdot 16} = \pm\sqrt{2 \cdot 4 \cdot 4} = \pm 4 \sqrt{2}$<br>
   $2x = -3 \pm 4 \sqrt{2}$<br>
   $x = \frac{-3 \pm 4 \sqrt{2}}{2}$<br>
3. $f(x) = (3x -2)^{2} + 75$<br>
   $(3x-2)^{2} = -75$<br>
   $3x -2 = \pm\sqrt{-75}$ --> No real solution - graph is not touching the x-axis<br>
   $3x -2 = \pm\sqrt{ -1 \cdot 25 \cdot 3} = 5i\sqrt{3}$
   $x = \frac{2 \pm 5i \sqrt{3}}{3}$ --> Complex conjugate in the complex form of $a +bi$<br>

>**Factoring by Diamond Method**

<img src="Images/diamond_method.svg" width="320"><br>

**Steps:**
1. Fill out the diamond.
   $b$ is the coefficient of $x$
   $a \cdot c$ is the product of the leading and constant coefficients
   $m$ such that $m + n = b$
   $n$ such that $m \cdot n = a \cdot c$
2. Solution is $ax^{2} + bx +c = ax^{2} + mx + nx + c$
3. Factor by grouping<br>
   $(ax^{2} + mx) + (nx+c)$<br>
   Factor out GCF<br>
   $x(ax +m) + 1(nx+c)$<br>
   If successful, the parenthesis match<br>
   $(ax +m)(x+n) = 0$

**Examples:**
1. $f(x) = x^{2} + 7x +6$<br>
   $x^{2} + 7x + 6 = 0$<br>
   $b = 7, a \cdot c = 6, m = 1, n = 6$<br>
   $x(x+1)+6(x+1) = 0$<br>
   $(x+1)(x+6) = 0$<br>
   $x=-1, x= -6$<br>
2. $h(x) = -12x +9 +4x^{2}$<br>
   $4x^{2} -12x +9 = 0$<br>
   $b = -12, a \cdot c = 36, m = -6, n = -6$<br>
   $(2x -3)^{2} = 0$
   $x = \frac{3}{2}$

>**Completing the Square**

1. $f(x)= x^{2} +4x -3$<br>
   $(x^{2} +4x) - 3 = 0$<br>
   $(x +2)^{2} -4 -3 =0$<br>
   $(x+2)^{2} - 7 = 0$<br>
2. $h(x) = 5x^{2} -10x +2$<br>
   $x^{2} - 2x + \frac{2}{5}$<br>
   $(x-1)^{2} - \frac{3}{5}=0$

>**Graphs of quadratics**

<img src="Images/Quadratic Solutions.png" width="420"><br>

$f(x) = ax^{2} + bx +c$<br>
$a>0$ Upward parabola<br>
$a<0$ Downward parabola<br>
y-intercept = (0,c)<br>
x-intercept: $ax^{2} + bx +c = 0$<br>
Vertex = $(\frac{-b}{2a}, f(x))$<br>
Vertex form: $f(x) = a(x + h)^{2} + k$

### Polynomial Functions

$f(x) = a_{n}x^{n} + a_{n-1}x^{n-1} + ... + a_{2}x^{2} + a_{1}x + a_0$<br>
leading term: $a_{n}x^{n}$, constant term: $a_0$<br>
Degree: $n$, largest exponent in polynomial
Domain is all $\mathbb{R}$

### Power Functions
Definition: Polynomial with only one term<br>
<img src="Images/powerfns.jpg" width="420">

