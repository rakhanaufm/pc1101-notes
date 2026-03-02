Muhammad Rakha Naufal Maulana A0330820U
# 1. Polarisation in Complex Notation
a)
We can first use the fact that two polarisation vectors that differ by a global phase, i.e., $\hat{\mathbf{e}}$ and $e^{i\phi} \hat{\mathbf{e}}$ with $\phi \in \mathrm{Re}$, describe the same polarisation. We can thus simplify $\alpha$ and $\beta$ into 
$$
\alpha = \cos\theta  \hat{\mathbf{e}}_{H}, \beta = \sin \theta  \hat{\mathbf{e}}_{V}
$$
We can see that,
$$
|\alpha|^{2} + |\beta|^{2} = \cos ^{2} \theta+ \sin ^{2}\theta = 1
$$
Which is consistent with the normalization.

b)
Take
$$
u = \begin{pmatrix}
\alpha \\
\beta
\end{pmatrix}
, v = \begin{pmatrix}
-\beta^\star \\
\alpha^\star 
\end{pmatrix}
$$
Using the given definition of scalar product,
$$
u \cdot v = \sum^2_{k=1} u_{k}^\star v_{k} =  \alpha^\star(-\beta^\star) + \beta^\star(\alpha^\star) = -\alpha^\star \beta^\star+\beta^\star \alpha^\star = 0
$$
Hence it is orthogonal.
To prove the uniqueness, let
$$
w = \begin{pmatrix}
x  \\
y
\end{pmatrix}
$$
with
$$
\alpha^\star x + \beta^\star y = 0
$$
solve
$$
x = -\beta^\star \lambda, y = \alpha^\star \lambda
$$
so
$$
w = \lambda \begin{pmatrix}
-\beta^\star \\
\alpha^\star
\end{pmatrix}
$$
Only freedom is global phase -> unique up to phase.
Q.E.D.

c)
Given
$$
\hat{e}_{\theta} = \begin{pmatrix}
\cos \theta \\
\sin \theta 
\end{pmatrix}
$$
Using result from part b, we have
$$
\hat{e}_{\perp } = \begin{pmatrix}
-\sin \theta \\
\cos \theta
\end{pmatrix}
$$
But
$$
\hat{e}_{\theta + \frac{\pi}{2}} = \begin{pmatrix}
\cos\left( \theta + \frac{\pi}{2} \right) \\
\sin\left( \theta + \frac{\pi}{2} \right)
\end{pmatrix} = \begin{pmatrix}
-\sin \theta \\
\cos \theta
\end{pmatrix}
$$
d)
Standard normalized vectors:
Right circular:
$$
\hat{e}_{R} = \frac{1}{\sqrt{ 2 }}\begin{pmatrix}
1 \\
-i
\end{pmatrix}
$$
Left circular:
$$
\hat{e}_{L} = \frac{1}{\sqrt{ 2 }}\begin{pmatrix}
1 \\
i
\end{pmatrix}
$$
Check orthogonality:
$$
e_{R}\cdot e_{L} = \frac{1}{2}(1^\star \cdot 1 + (-i)^\star \cdot i) = \frac{1}{2}(1 + i^{2}) = \frac{1}{2}(1-1) = 0
$$
# 2. Double-slit with finite apertures
We observe two effects happening, the single slit diffraction and the double slit interference. Fraunhofer diffraction gives,
$$
A_{\text{single}} \propto \frac{\sin \beta}{\beta}, \beta = \frac{\pi a\sin \theta}{\lambda}
$$
While the double slit phase difference is,
$$
\delta = \frac{2\pi d}{\lambda}\sin \theta
$$
This gives the total amplitude to be:
$$
A \propto \frac{\sin \beta}{\beta}(e^{i\delta/2}+e^{-i\delta/2}) = 2 \frac{\sin \beta}{\beta}\cos\left( \frac{\delta}{2} \right)
$$
the intensity is just amplitude squared so we have:
$$
I = I_{0}\left( \frac{\sin\beta}{\beta} \right)^{2} \cos ^{2}\left( \frac{\pi d}{\lambda}\sin \theta \right)
$$
Or,
$$
I(\theta) = I_{0}\left(\frac{\sin\left( \frac{\pi a}{\lambda}\sin \theta  \right)}{\frac{\pi a}{\lambda}\sin \theta}\right)^{2} \cos ^{2}\left( \frac{\pi d}{\lambda}\sin \theta \right)
$$
with $I_{0}$ the intensity at the center
# 3. Is Your Phone's Camera Diffraction Limited?
a)
Rayleigh criterion:
$$
\theta_{min} = 1.22 \frac{\lambda}{D}
$$
Using the small angle approximation, we have
$$
\theta \approx \frac{s}{R}, s=1 \text{mm}
$$
So,
$$
R_{max} = \frac{sD}{1.22 \lambda}
$$
For $\lambda$ im going to use 550 nm and I measured $D$ to be 
around 4 mm. substituting into the equation gives,
$$
R_{max} \approx 6 \space m
$$

b)
The largest distance where ticks are still resolvable is about 3 meters from the lens to the ruler.
1 meter:
![[WhatsApp Image 2026-02-11 at 22.17.22.jpeg]]
2 meter:
![[WhatsApp Image 2026-02-11 at 22.17.21.jpeg]]
3 meter:
![[WhatsApp Image 2026-02-11 at 22.17.21(1).jpeg]]
The images in order are from distance $D$ = 1, 2, 3 meters respectively. I was unable to distinguish between the mm lines after 3 meters. Here, I obtain $R_{max}$ to be lower than the theoretical limit, and I suspect that the discrepancies are from:
1. Sensor resolution 
2. Image processing 
3. Aberrations 
4. Hand shake 
5. Finite pixel size