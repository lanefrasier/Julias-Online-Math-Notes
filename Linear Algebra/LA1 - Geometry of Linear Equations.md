# Geometry of Linear Equations
[PDF](Linear%Algebra\PDFs\Geometry%of%Linear%Equations.pdf)

## Contents

[Definitions](#Definitions)<br>


### Definitions

### Vectors

vector - magnitude and direction
Ex. velocity
$\vec{v} = (5, 0) = 
\begin{bmatrix} 5 \\ 0 \end{bmatrix} = \begin{bmatrix} x \\ y \end{bmatrix}$

$\mathbb{R}^2$ = real coordinate space (2D) All possible real-valued 2-tuple

### Adding Vectors/Matrices

Geometrically:<br>
<img src="Images/vector_addition.png" width="420"><br>
Computationally:<br>
<img src="Images/AddingMatrix.png" width="420"><br>

Scalar multiples have the same direction and are parallel lines<br>
$\vec{a} = \begin{bmatrix} 2 \\ 1 \end{bmatrix} \qquad || \qquad 3\vec{a} = \begin{bmatrix} 6 \\ 3 \end{bmatrix} = 3 \begin{bmatrix} 2 \\ 1 \end{bmatrix} \qquad || \qquad -1\vec{a} = \begin{bmatrix} -2 \\ -1 \end{bmatrix}$

Magnitude: magnitude of original $\vec{v} \cdot |{scalar}| = ||c\cdot \vec{v}|| = |c| \cdot ||\vec{v}||$<br>
Direction: opposite directions are 180$^{\circ}$

> Unit Vectors

$\hat{i} = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix} \qquad \hat{j} = \begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix} \qquad \hat{k} = \begin{bmatrix} 0 \\ 0 \\ 1\end{bmatrix}$<br>
Unit $\vec{v}$ in any direction of $\vec{v}$ with magnitude of 1<br>
$\dfrac{\vec{v}}{||\vec{v}||}$

### Linear Combination

$S = v_{1}, v_{2}, ..., v_{n}$ in $\mathbb{R}$ is linearly dependent if and only if $c_{1} v_{1}, c_{2} v_{2}, ..., c_{n}v_{n}$ in $\mathbb{R} = 0$ for some $c_{i}$ where at least one is non-zero.

**Proof**

Assume $c_1 \neq 0$<br>
$v_{1} + \dfrac{c_2}{c_1}v_2 + ... + \dfrac{c_n}{c_1}v_n = 0$<br>
$v_1 = -\dfrac{c_2}{c_1}v_2 - ... - \dfrac{c_n}{c_1}v_n$<br>
Since $v_1$ can be written as a combination of the other vectors which are non-zero, it must be linearly dependent.