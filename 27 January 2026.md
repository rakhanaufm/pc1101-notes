# Normalise Gaussians
Use the formula
$$
\int_{-\infty}^{\infty} e^{-u^{2}} \, du = \sqrt{ \pi } 
$$
To find the normalization factor $A(a)$ of a Gaussian
$$
G(x) = A(a)e^{-\frac{(x-x_{0})^{2}}{2a^{2}}}
$$
Example:
$$
1=\int_{-\infty}^{\infty} G(x) \, dx  = \int_{-\infty}^{\infty} Ae^{-\frac{(x-x_{0})^{2}}{2a^{2}}} \, dx 
$$
let $u = \frac{x-x_{0}}{\sqrt{ 2 }a}$
$$
=A\int_{-\infty}^{\infty} a\sqrt{ 2 }e^{-u^{2}} \, du 
$$
$$
=Aa\sqrt{ 2 }\sqrt{ \pi }
$$
$$
A=\frac{1}{\sqrt{ 2\pi }a}
$$

## Average Position of the Gaussian Wave:
$$
\langle x \rangle =x_{0}
$$
Here average of $f(x)$ is defined as
$$
\langle f(x) \rangle \equiv \int_{-\infty}^{\infty} f(x)G(x) \, dx 
$$
Hence,
$$
\langle x \rangle = \int_{-\infty}^{\infty} xG(x) \, dx 
$$
$$
=\int_{-\infty}^{\infty} x \frac{1}{\sqrt{ 2\pi }a}e^{-\frac{(x-x_{0})^2}{2a^{2}}} \, dx 
$$
$$
=\int_{-\infty}^{\infty} [(x-x_{0})+x_{0}]  \frac{1}{\sqrt{ 2\pi }a}e^{-\frac{(x-x_{0})^{2}}{2a^{2}}}\, dx 
$$
$$
\langle x \rangle =\frac{1}{\sqrt{ 2\pi }a}\int_{-\infty}^{\infty} (x-x_{0})e^{-\frac{(x-x_{0})^{2}}{2a^{2}}} \, dx + \frac{x_{0}}{\sqrt{ 2\pi }a}\int_{-\infty}^{\infty} e^{-\frac{(x-x_{0})^{2}}{2a^{2}}} \, dx  
$$
let $w=x-x_0$
$$
= \frac{1}{\sqrt{ 2\pi }a} \int_{-\infty}^{\infty} we^{-\frac{w^{2}}{2a^{2}}} \, dw + x_{0}\int_{-\infty}^{\infty} G(x) \, dx 
$$
The first term amounts to zero because the integral is even but the term itself is odd, and for the second term we get that its equal to 1 from normalization
$$
=x_{0}
$$
Q.E.D.

## Variation of the Gaussian Wave:
$$
\langle (x-x_{0})^{2} \rangle = a^{2}
$$
Proof:
$$
\langle (x-x_{0})^{2} \rangle = \int_{-\infty}^{\infty} (x-x_{0})^{2}G(x) \, dx 
$$
$$
=\frac{1}{\sqrt{ 2\pi }a}\int_{-\infty}^{\infty} (x-x_{0})^{2}e^{-\frac{(x-x_{0})^{2}}{2a^{2}}} \, dx 
$$
Let $w = x-x_0$
$$
= \frac{1}{\sqrt{ 2\pi }a}\int_{-\infty}^{\infty} w^{2}e^{-\frac{w^{2}}{2a^{2}}} \, dw
$$
$$
\frac{d}{dw}e^{-\frac{w^{2}}{2a^{2}}}=e^{-\frac{w^{2}}{2a^{2}}} \frac{d}{dw}\left( -\frac{w^{2}}{2a^{2}} \right)
$$
$$
=-\frac{2w}{2a^{2}}e^{-\frac{w^{2}}{2a^{2}}}
$$
$$
=-\frac{w}{a^{2}}e^{-\frac{w^{2}}{2a^{2}}}
$$
The integral becomes,
$$
=-\frac{a}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty} w(e^{-\frac{w^{2}}{2a^{2}}}) \, dw
$$
$$
\langle (x-x_{0})^{2} \rangle = -\frac{a}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty} w(e^{-\frac{w^{2}}{2a^{2}}}) \, dw 
$$
Integration by parts
$$
\frac{d}{dx}(uv)=u'v+uv'
$$
$$
\Rightarrow uv' = \frac{d}{dx}(uv) - u'v
$$
$$
\int \Rightarrow \int dxuv'=\int dx \frac{d}{dx}uv - \int dxu'v
$$
$$
\int dxuv' = uv - \int dxu'v
$$
Hence,
$$
\langle (x-x_{0})^{2} \rangle = -\frac{a}{\sqrt{ 2\pi }}we^{-\frac{w^{2}}{2a^{2}}}|^{\infty}_{-\infty} + \frac{a}{\sqrt{ 2\pi }}\int dxe^{-\frac{w^{2}}{2a^{2}}}
$$
$$
= 0 + a^{2}\int du \frac{1}{\sqrt{ 2\pi }a}e^{-\frac{w^{2}}{2a^{2}}} = a^{2}
$$

# Waves in 3D
## Monochromatic Plane Waves
A monochromatic plane wave is given by
$$
A\cos(\mathbf{k}\cdot \mathbf{x} - \omega t + \phi)
$$
Wave vector: $\textbf{k}=k\hat{\mathbf{e}}_k$ carries magnitude and direction
Propagates in direction of $\textbf{k}$
Dispersion relation: $\omega = c|\textbf{k}|$ 
Wavefronts: Planes perpendicular to $\hat{\mathbf{e}}_k$

## Why Plane Waves Matter
Basis functions: Every wave can be decomposed as sum of plane waves
Beam modeling: Waves propagating in $\textbf{z}$-direction is described by:
$$
f(\mathbf{x},t)\propto G(x,y)\cos(k\mathbf{z}-\omega t)
$$
Profile examples:
	Cylindrical beam: Step function (unrealistic)
$$
G(x,y) \propto \begin{cases}
1, x^{2}+y^{2} \leq a^{2} \\
0, x^{2}+y^{2} > a^{2}
\end{cases}
$$
	Gaussian beam: $G(x,y) \propto e^{-\frac{(x^{2}+y^{2})}{4a^{2}}}$ (realistic)

# Polarisation
Electric field is a vector
Light is a transverse wave: $\textbf{E}$ perpendicular to propagation direction
Polarisation: Direction of electric field oscillation
Define orthogonal unit vectors in transverse plane:
	$\hat{\textbf{e}}_H$ (horizontal) and $\hat{\textbf{e}}_V$ (vertical)
Such that $\hat{\mathbf{e}}_{H} \times \hat{\mathbf{e}}_{V}= \hat{\mathbf{e}}_{k}$

## Linear Polarisation
Electric field oscillates along fixed direction:
$$
\mathbf{E}(\mathbf{x},t)=E_{0}\cos(k\mathbf{z}-\omega t+\phi)
$$
Where: $\hat{\mathbf{e}}_{\theta} \equiv \cos \theta \hat{\mathbf{e}}_{H}+\sin \theta \hat{\mathbf{e}}_{V}$
Field oscillates along direction $\theta$
Note: $\theta'= \theta + \pi$ gives same polarisation
Most common type in everyday applications

## Circular Polarisation
Electric field **rotates** around propagation axis
$$
\mathbf{E}(\mathbf{x},t) = \frac{E_{0}}{\sqrt{ 2 }}[\cos (k\mathbf{z}-\omega t+\phi)\hat{\mathbf{e}}_{H} \pm \sin (k\mathbf{z}-\omega t+\phi) \hat{\mathbf{e}}_{V}]
$$
Right-handed: - sign
	(counterclockwise from receiver view)
Left-handed: + sign
	(clockwise from receiver view)
Factor $1/\sqrt{ 2 }$  ensures proper normalisation

## Elliptical Polarisation
Most general form:
$$
\mathbf{E}(\mathbf{x},t) = \frac{E_{0}}{\sqrt{ 2 }}[\cos \theta\cos (k\mathbf{z}-\omega t+\phi_{1})\hat{\mathbf{e}}_{H} + \sin \theta\sin (k\mathbf{z}-\omega t+\phi_{2}) \hat{\mathbf{e}}_{V}]
$$
Special cases:
$$
(\theta, \phi_{1},\phi_{2}) = \begin{cases}
(\theta,\phi,\phi), &\text{Linear} \\
\left( \frac{\pi}{4}, \phi, \phi + \frac{\pi}{2} \right), &\text{Circular right} \\
\left( \frac{\pi}{4}, \phi, \phi - \frac{\pi}{2} \right), &\text{Circular left}
\end{cases}
$$
Verify $(\theta, \phi, \phi)$ means linear
$$
\begin{align}
\mathbf{E}(\mathbf{x},t)&=E_{0}\cos \theta \cos(kz-\omega t+\phi)\hat{e}_{H}+\sin \theta \cos(kz-\omega t+\phi)\hat{e}_{V} \\
&=E_{0}\cos(kz-\omega t+\phi)[\cos \theta \hat{e}_{H}+\sin \theta \hat{e}_{V}] \\
&=E_{0}\hat{e}_{\theta}\cos(kz-\omega t+\phi)
\end{align}
$$
Linear polarisation in $\theta$-direction or $\theta'=\theta+\pi$ 

