Muhammad Rakha Naufal Maulana A0330820U
# 1. Matrix Form of Lorentz Transformation
a)
$$
\mathbf{A}^T\eta \mathbf{B} = 
\begin{pmatrix}
A_{t} & A_{x}
\end{pmatrix}
\begin{pmatrix}
-1 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
B_{t} \\
B_{x}
\end{pmatrix}
$$
$$
= 
\begin{pmatrix}
A_{t} & A_{x}
\end{pmatrix}
\begin{pmatrix}
-B_{t} \\
B_{x}
\end{pmatrix}
$$
$$
A^T \eta \mathbf{B} = - A_{t}B_{t} + A_{x}B_{x}
$$
which is indeed equivalent
b)
We want to show that
$$
(\mathbf{\Lambda}\mathbf{A})^T\eta (\mathbf{\Lambda}\mathbf{B}) = \mathbf{A}^T \eta \mathbf{B}
$$
and the key idea is that
$$
(\mathbf{\Lambda}\mathbf{A})^T \eta (\mathbf{\Lambda}\mathbf{B}) = \mathbf{A}^T (\mathbf{\Lambda}^T \eta \mathbf{\Lambda})\mathbf{B}
$$
So it suffices to prove
$$
\mathbf{\Lambda}^T \eta \mathbf{\Lambda} = \eta
$$
The Lorentz matrix is
$$
\mathbf{\Lambda}
=
\begin{pmatrix}
\cosh \rho & -\sinh \rho \\
-\sinh \rho & \cosh \rho
\end{pmatrix}
$$
Note that it's symmetric which means its transpose is itself
Let's do this
$$
\eta \mathbf{\Lambda} = 
\begin{pmatrix}
-1 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\cosh \rho & -\sinh \rho \\
-\sinh \rho & \cosh \rho
\end{pmatrix}
= 
\begin{pmatrix}
-\cosh \rho & \sinh \rho \\
-\sinh \rho & \cosh \rho
\end{pmatrix}
$$
Now let's multiply it by its transpose
Top left is
$$
\cosh \rho(-\cosh \rho) + (-\sinh \rho)(-\sinh \rho)= -\cosh ^{2}\rho + \sinh ^{2} \rho = -1
$$
Top right is
$$
\cosh \rho(\sinh \rho) + (-\sinh \rho)(\cosh \rho) = 0
$$
Bottom left is
$$
(-\sinh \rho)(-\cosh \rho) + \cosh \rho(-\sinh \rho) = 0
$$
Bottom right is
$$
(-\sinh \rho)(\sinh \rho) + \cosh \rho(\cosh \rho) = -\sinh ^{2}\rho + \cosh ^{2}\rho = 1
$$
So
$$
\mathbf{\Lambda}^T \eta \mathbf{\Lambda} = 
\begin{pmatrix}
-1 & 0 \\
0 & 1
\end{pmatrix}
=
\eta
$$
# 2. Pauli Matrices
a)
To find the eigenvalues we use the equation
$$
(\mathbf{M}- \lambda \mathbf{I}) = 0
$$
and impose that the determinant must be zero
$\sigma_{x}$:
$$
\begin{vmatrix}
-\lambda & 1 \\
1 & -\lambda
\end{vmatrix}
= \lambda^{2} -1 =0 \to \lambda = \pm 1
$$
which has eigenvectors
$\lambda = +1$
$$
\begin{pmatrix}
1 \\
1
\end{pmatrix}
$$
$\lambda=-1$
$$
\begin{pmatrix}
1 \\
-1
\end{pmatrix}
$$
$\sigma_{y}$:
$$
\begin{vmatrix}
-\lambda & -i \\
i & -\lambda
\end{vmatrix}
= \lambda^{2} -1 = 0
\to \lambda = \pm 1
$$
which has eigenvectors
$\lambda=+1$
$$
\begin{pmatrix}
1 \\
i
\end{pmatrix}
$$
$\lambda=-1$
$$
\begin{pmatrix}
1 \\
-i
\end{pmatrix}
$$

$\sigma_{z}$:
$$
\begin{vmatrix}
1-\lambda & 0 \\
0 & -1-\lambda
\end{vmatrix}
= 1- \lambda^{2} = 0 \to \lambda = \pm 1
$$
which has eigenvectors
$\lambda = +1$
$$
\begin{pmatrix}
1 \\
0
\end{pmatrix}
$$
$\lambda = -1$
$$
\begin{pmatrix}
0 \\
1
\end{pmatrix}
$$
b)
$$
\mathbf{M} =
\begin{pmatrix}
C_{0} + C_{3} & C_{1} -iC_{2} \\
C_{1} + iC_{2} & C_{0}-C_{3}
\end{pmatrix}
$$
Thus, rewriting in terms of the matrix elements, we have
$$
C_{1} = \frac{\mathbf{M}_{1,2} + \mathbf{M}_{2,1}}{2}, C_{0} = \frac{\mathbf{M}_{1,1} + \mathbf{M}_{2,2}}{2},C_{3} = \frac{\mathbf{M}_{1,1} - \mathbf{M}_{2,2}}{2}, C_{2} = \frac{\mathbf{M}_{2,1}- \mathbf{M}_{1,2}}{2i}
$$
c)
$\mathbf{M}^{\dagger}$ is
$$
\mathbf{M}^{\dagger}=
\begin{pmatrix}
(C_{0}+C_{3})^\star & (C_{1}+iC_{2})^\star \\
(C_{1}-iC_{2})^\star & (C_{0}-C_{3})^\star
\end{pmatrix}
=
\begin{pmatrix}
C_{0}^\star + C_{3}^\star & C_{1}^\star-iC_{2}^\star \\
C_{1}^\star+iC_{2}^\star & C_{0}^\star - C_{3}^\star
\end{pmatrix}
$$
as this must be equal to $\mathbf{M}$, we have
$$
C_{0}^\star+C_{3}^\star = C_{0} + C_{3}, C_{0}^\star - C_{3}^\star = C_{0}-C_{3}
$$
which implies
$$
C_{0}^\star = C_{0}, C_{3}^\star = C_{3}
$$
and
$$
C_{1}^\star - iC_{2}^\star = C_{1} - iC_{2}, C_{1}^\star + iC_{2}^\star = C_{1} + iC_{2}
$$
which implies
$$
C_{1}^\star = C_{1}, C_{2}^\star = C_{2}
$$
this means
$$
C_{0},C_{1},C_{2},C_{3} \in \mathbb{R}
$$
