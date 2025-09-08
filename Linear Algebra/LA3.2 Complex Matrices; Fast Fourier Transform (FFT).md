# Complex Matrices; Fast Fourier Transform (FFT)
[Complex Matrices; Fast Fourier Transform (FFT) (PDF)](PDFs/3.2%20Complex%20Matrices,%20fast%20Fourier%20transformation.pdf)

## Contents

[Definitions](#Definitions)<br>


### Definitions

### Complex Matrices

Diagonalize A by constructing its eigenvalue matrix $\Lambda$ and eigenvector matrix S.<br>
$$
A = \begin{bmatrix} 2 & 1-i \\\\ 1+i & 3 \end{bmatrix} = \bar{A}^{T} = A^{H}
$$

1. Diagonalize the matrix
det$(A-\lambda I) = 0$<br>
$$
det \begin{vmatrix} 2-\lambda & 1-i \\\\ 1+i & 3-\lambda \end{vmatrix} = 0
$$

$(2-\lambda)(3-\lambda) - (1+i)(1-i) = 0$<br>
$6-5\lambda + \lambda^2 - 2 = 0$<br>
$\lambda^2 - 5\lambda + 4 = 0$<br>
$(\lambda-1)(\lambda-4) = 0$<br>
$\lambda = 1, 4$
Hermetian matrices always have real eigenvalues

2. Find eigenvectors

$\lambda = 1$:<br>
$(A-\lambda I)v = 0$ -> should be singular<br>
$$
\begin{bmatrix} 1 & 1-i \\\\ 1+i & 2 \end{bmatrix} \begin{bmatrix} v_1 \\\\ v_2 \end{bmatrix} = 0
$$

Second row is always a constant multiple of the first row, must be linearly dependent. Multiple through by $1+i$<br>
$v_1 = (1-i)$<br>
$v_2 = -1$<br>
$$
v = \begin{bmatrix} 1-i \\\\ -1 \end{bmatrix}
$$

$\lambda = 4$<br>
$(A-\lambda I)u = 0$ -> should be singular<br>
$$
\begin{bmatrix} -2 & 1-i \\\\ 1+i & -1 \end{bmatrix} \begin{bmatrix} u_1 \\\\ u_2 \end{bmatrix} = 0
$$

Second row is always a constant multiple of the first row, must be linearly dependent. Multiple through by $1+i$<br>
$u_1 = 1$<br>
$u_2 = 1 + i$<br>
$$
u = \begin{bmatrix} 1 \\\\ 1+i \end{bmatrix}
$$

u and v are orthogonal when conjugate elements and dot them together.<br>
$$
\bar{v}^T u = \begin{bmatrix} (1+i) & - 1 \end{bmatrix} \begin{bmatrix} 1 \\\\ 1 +i \end{bmatrix} = 0
$$$

3. Construct matrices $\Lambda$ and S
$$
\Lambda = \begin{bmatrix} 1 & 0 \\\\ 0 & 4 \end{bmatrix}
$$

Normalize u and v, multiply by length:<br>
$$
S = \dfrac{1}{\sqrt{3}} \begin{bmatrix} 1-i & 1 \\\\ -1 & 1+i \end{bmatrix}
$$
S is now unitary -> $S^-1 = \bar{S}^{T}$<br>
$A = S\Lambda S^-1 = S\Lambda \bar{S}^T$<br>
$$
A = \dfrac{1}{\sqrt{3}} \begin{bmatrix} 1-i & 1 \\\\ -1 & 1+i \end{bmatrix} \begin{bmatrix} 1 & 0 \\\\ 0 & 4 \end{bmatrix} \dfrac{1}{\sqrt{3}} \begin{bmatrix} 1+i & -1 \\\\ 1 & 1-i \end{bmatrix}
$$