# Symmetric Matrices and Positive Definiteness
[Symmetric Matrices and Positive Definiteness (PDF)](PDFs/3.1%20Symmetric%20Matrices%20and%20positive%20definiteness.pdf)

## Contents

[Definitions](#Definitions)<br>


### Definitions

### Positive Definite Matrices

Explain why each of the following is true:

1. Every positive definite matrix is invertible

A invertible <-> det A = $\lambda_1 \cdot \lambda_2 \cdot ... \cdot \lambda_n \neq 0$<br>
Where $\lambda_1, ..., \lambda_n$ are the eigenvalues of A.

A is positive definite <-> $\lambda_1, ..., \lambda_n > 0$

det A = $\lambda_1 \cdot \lambda_2 \cdot ...\cdot \lambda_n >0 \neq 0$

2. The only positive definite projection matrix is P=I

P is projection <-> Eigenvalues of P = 0 or = 1<br>
P is positive definite <-> eigenvalues > 0<br>

Eigenvalues of P must be = 1<br>
Only matrix with Eigenvalues = 1 and symmetric must be Identity matrix

Optional proof:<br>
If P is diagonalizeable (every symmetric matrix is diagonalizeable) -> $P = UI U^{-1}$ -> $P = U U^{-1} = I$<br>

3. D is diagonal with positive entries is positive definite

D = diag($d_1 d_2 ... d_n$)<br>

One way to show positive definite:<br>
For any vector $x \neq$, $x^{T}Dx>0$<br>
$x = x_1 x_2 ... x_n$<br>
$x^{T}Dx = d_1 x_1^2 + d_2 x_2^2 + ... + d_n x_n^2$<br>
By definition, each $d$ is positive, every square is positive, result must $>0$

Other way to prove:<br>
diagonals are positive, and we know that the diagonals are the eigenvalues. All must be positive, which proves positive definite.

4. S symmetric with det S>0 might not be positive definite
$$
S = \begin{bmatrix} -3 & 1 \\\\ 1 & -2 \end{bmatrix}
$$

det S = 5 > 0<br>
S not positive definite.<br>

If we look at the -3<br>
$x^{T}Sx -> x = (1 \quad 0)^{T}$<br>
We know this must be positive for every value of x<br>
$x^{T}Sx = -3$ Not positive