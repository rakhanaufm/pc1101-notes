Muhammad Rakha Naufal Maulana A0330820U
# 1. Gaussian Amplitudes
a) Compute the normalisation constant A

For a Gaussian amplitude, the normalization is
$$
\int_{-\infty}^{\infty} |G(x)|^{2} \, dx =1
$$
Substituting the given form for $G(x,t)$ we get,
$$
\int_{-\infty}^{\infty} \left(Ae^{-\frac{(x-ct)^{2}}{4a^{2}}}e^{i(k_{0}x-\omega_{0}t)}\right)^{2} \, dx =1
$$
We can separate the expression from the phase term:
$$
\left(Ae^{-\frac{(x-ct)^{2}}{4a^{2}}}e^{i(k_{0}x-\omega_{0}t)}\right)^{2} = A^{2}e^{-\frac{(x-ct)^{2}}{2a^{2}}}e^{i(2k_{0}x-2\omega_{0}t)}
$$
$$
e^{i(2k_{0}x-2\omega_{0}t)}A^2\int_{-\infty}^{\infty} e^{-\frac{(x-ct)^{2}}{2a^{2}}} \, dx =1
$$
As the phase term doesn't contribute to the normalization, we can omit them from the calculations,
$$
A^{2}\int_{-\infty}^{\infty} e^{-\frac{(x-ct)^{2}}{2a^{2}}} \, dx = 1
$$
Using the property of the Gaussian integral,
$$
\int_{-\infty}^{\infty} e^{-a(x+b)^{2}} \, dx = \sqrt{ \frac{\pi}{a} } 
$$

We get,
$$
A^2\sqrt{ 2\pi a^{2} }=1
$$
Solve for $A$
$$
A^{2}=\frac{1}{\sqrt{ 2\pi a^{2} }}
$$
Or,
$$
A=\frac{1}{\sqrt{\sqrt{ 2\pi a^{2} }}}
$$


b) Show that the centre of the wave packet, i.e., the average position $x_{0}(t)= \langle x_{0} \rangle(t)$, moves at the speed of light $c$.

Using the given definition of the spatial average of a field, we get
$$
\langle x \rangle (t) = \int_{-\infty}^{\infty} x\left(Ae^{-\frac{(x-ct)^{2}}{4a^{2}}}e^{i(k_{0}x-\omega_{0}t)}\right)^{2} \, dx 
$$
$$
=A^{2}\int_{-\infty}^{\infty} xe^{-\frac{2(x-ct)^{2}}{4a^{2}}} \, dx 
$$
We can compute the integral using integration by parts,
$$
=\int_{-\infty}^{\infty} x \frac{1}{\sqrt{ 2\pi }a}e^{-\frac{(x-ct)^2}{2a^{2}}} \, dx 
$$
$$
=\int_{-\infty}^{\infty} [(x-ct)+ct]  \frac{1}{\sqrt{ 2\pi }a}e^{-\frac{(x-ct)^{2}}{2a^{2}}}\, dx 
$$
$$
\langle x \rangle =\frac{1}{\sqrt{ 2\pi }a}\int_{-\infty}^{\infty} (x-ct)e^{-\frac{(x-ct)^{2}}{2a^{2}}} \, dx + \frac{ct}{\sqrt{ 2\pi }a}\int_{-\infty}^{\infty} e^{-\frac{(x-ct)^{2}}{2a^{2}}} \, dx  
$$
let $w=x-ct$
$$
= \frac{1}{\sqrt{ 2\pi }a} \int_{-\infty}^{\infty} we^{-\frac{w^{2}}{2a^{2}}} \, dw + ct\int_{-\infty}^{\infty} |G(x)|^{2} \, dx 
$$
The first term amounts to zero because the integral is even but the term itself is odd, and for the second term we get that its equal to 1 from normalization
$$
\langle x \rangle = ct = x_{0}
$$
Q.E.D.

c) Prove that the Gaussian wave packet does not disperse by showing that the variation $\langle (x-x_{0})^{2} \rangle(t)$ is independent of time

Again using the definition given in the problem statement, we have
$$
\langle (x-x_{0})^{2} \rangle (t) = \int_{-\infty}^{\infty} (x-x_{0})\left(Ae^{-\frac{(x-ct)^{2}}{4a^{2}}}e^{i(k_{0}x-\omega_{0}t)}\right)^{2} \, dx 
$$
$$
=\frac{1}{\sqrt{ 2\pi }a}\int_{-\infty}^{\infty} (x-ct)^{2}e^{-\frac{(x-ct)^{2}}{2a^{2}}} \, dx 
$$
Let $w = x-ct$
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
\langle (x-ct)^{2} \rangle = -\frac{a}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty} w(e^{-\frac{w^{2}}{2a^{2}}}) \, dw 
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
which is a constant that is independent of time.

# 2. Plots of Gaussian Waves
a)![[Pasted image 20260127161924.png]]

b)
![[Pasted image 20260127162100.png]]
