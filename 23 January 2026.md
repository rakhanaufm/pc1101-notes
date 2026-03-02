# Forced Oscillation
Oscillation with damping and a driving term
$$
\ddot{f}(t) + 2 \beta \dot{f}(t) + \omega_{0}^2f(t) = D_{0}\cos(\omega t)
$$
It is an inhomogeneous linear differential equation
Solution:
$$
f(t) = f_{homo}(t) + f_{sp}(t)
$$
where $f_{homo}(t)$ is the solution of corresponding homogeneous equation:
$$
f_{homo}(t) = C_{1}e^{-\beta t}e^{i\omega t} + C_{2}e^{-\beta t}e^{-i\omega t}
$$
It is negligible in the long term because $f_{{homo}(t)}$ as $t \rightarrow \infty$

Special Solution
$f_{sp}(t)$ is one special solution that satisfies the whole equation:
$$
\ddot{f_{sp}} + 2\beta \dot{f_{sp}}(t) + \omega_{0}^2f_{sp}(t) = D_{0}\cos(\omega t)
$$
Guess that $f_{sp}(t) = a \cos(\omega t) + b\sin(\omega t)$ then solve for $a$ and $b$.
Alternative form: $f_{sp}(t) = A\cos(\omega t+\phi)$
Where $A = \sqrt{ a^2+b^2 } = \frac{D_{0}}{\sqrt{ 4\beta^2\omega^2 + (\omega^2 -\omega^2)^2}}$ and $\tan \phi = -\frac{b}{a} = \frac{2\beta \omega}{\omega^2-\omega_{0}^2}$
Resonance occurs at $\omega = \omega_{r} \equiv \sqrt{ \omega_{0}^2 - 2\beta^2 }$
For small damping, $\omega \approx \omega_{0}$

## Derivation of the Special Solution
$$
f_{sp} = a \cos(\omega t) + b\sin(\omega t) \Rightarrow \dot{f_{sp}} = -a \omega \sin(\omega t) + b \omega \cos(\omega t)
$$
$$
\Rightarrow \ddot{f_{sp}} = -a\omega^2\cos(\omega t) -b\omega^2\sin(\omega t) = -\omega^2f_{sp}
$$
$$
\text{ODE} \Rightarrow \ddot{f_{sp}} + 2 \beta \dot{f_{sp}} + \omega_{0}^2f_{sp} = -a\omega^2\cos(\omega t) -b\omega^2\sin(\omega t) -2\beta a\omega \sin(\omega t) + 2\beta \omega \cos(\omega t) + a\omega_{0}^2\cos(\omega t) +b\omega_{0}^2\sin(\omega t)
$$
$$
= [-a\omega^2 + 2\beta b\omega + a \omega_{0}^2]\cos(\omega t) = [-b\omega^2 -2\beta a \omega + b \omega_{0}^2]\sin(\omega t) = D_{0}\cos(\omega t)
$$
$$
\Rightarrow -a\omega^2 + 2\beta b \omega + a\omega_{0}^2 = D_{0}
$$
$$
-b\omega^2 -2\beta a \omega + b \omega_{0}^2 = 0
$$
$$
A = \frac{(\omega_{0}^2-\omega^2)D_{0}}{(\omega^2-\omega_{0}^2)^2+4\beta^2\omega^2}
$$
$$
B = \frac{2 \beta \omega D_{0}}{(\omega^2-\omega_{0}^2)^2+4\beta^2\omega^2}
$$
# Fourier Transform
Not all oscillations are simple harmonic
*Fundamental Principle*: Every oscillation can be written as superposition of single-frequency (simple harmonic) oscillations
$$
f(t) = \frac{1}{\sqrt{ 2 \pi }}\int_{-\infty}^{\infty} \tilde{f}(\omega)e^{i\omega t} \, d\omega
$$
Fourier transform is the "weight" of each frequency component
$$
\tilde{f}(\omega) \equiv \frac{1}{\sqrt{ 2 \pi }} \int_{-\infty}^{\infty} f(t) e^{-i\omega t} \, dt 
$$
For Fourier transform to exists, it requires that
$$
\int_{-\infty}^{\infty} |f(t)|^2 \, dt 
$$

## Example 1
Prove that the Fourier transform of the square
$$
f(t) = \begin{cases}
A, &  -\frac{a}{2} \leq t \leq \frac{a}{2} \\ 
0 , & otherwise 
\end{cases}
$$
is a cardinal sine function
$$
\begin{align}
\tilde{f}(\omega) & = \frac{1}{\sqrt{ 2 \pi }}\int_{-\infty}^{\infty} f(t)e^{-i\omega t} \, dt \\
& = \frac{1}{\sqrt{ 2 \pi }}\int_{-\frac{a}{2}}^{a/2} Ae^{-i\omega t} \, dt  \\
& = \frac{A}{\sqrt{ 2 \pi }}  \frac{1}{-i\omega}e^{-i\omega t}|^{\frac{a}{2}}_{-\frac{a}{2}} \\
& = \frac{\frac{A}{\sqrt{ 2 \pi } }1}{-i\omega}[e^{-i\omega a/2 }-e^{i\omega a/2}] \\
& = \frac{2A}{\sqrt{ 2 \pi }\omega}\sin\left( \frac{\omega a}{2} \right) \\
& = \frac{\frac{aA}{\sqrt{ 2 \pi }}\sin\left( \frac{\omega a}{2} \right)}{\frac{\omega a}{2}} \\
& = \frac{aA}{\sqrt{ 2 \pi }}sinc \left( \frac{\omega a}{2} \right)
\end{align}
$$

# Waves in 1D and Superposition
## Waves
For a wave travelling at speed $c$ in the positive $x$-direction without deformation:
$$
f(x,t) = f(x-ct,0)
$$
It satisfies a linear **wave equation** :
$$
\frac{\partial^2f}{\partial t^{2}} = c^{2} \frac{\partial^{2}f}{\partial x^{2}}
$$Monochromatic wave:
$$
\begin{align}
f(x,t) &= A\cos\left[ \frac{\omega}{c}(x-ct) + \phi \right] \\
&=A\cos(kx - \omega t + \phi)
\end{align}

$$
### Wave Number
$k$ is the wave number:
$$
|k| = \frac{\omega}{c} = \frac{2\pi}{\lambda}
$$
	Units: 1/m
	Sign of $k$ determines propagation direction
Here $\lambda$ is the wavelength
A few simple relations:
$$
c= \frac{\lambda}{t}=\lambda \nu=\frac{\omega}{k}
$$
### Amplitude and Intensity
Electric field of electromagnetic wave:
$$
E(x,t) = E_{0}\cos(kx-\omega t+\phi)
$$
	Amplitude $E_0$, Units: V/m for electric field
Instantaneous intensity:
$$
I(x,t) \equiv c \epsilon_{0}|E(x,t)|^2 = c \epsilon_{0}E_{0}^{2}\cos ^{2}(kx-\omega t+\phi)
$$
Light Intensity:
$$
I(x) \equiv <I(x,t)>_{t} = \frac{1}{2}c\epsilon_{0}E_{0}^{2}
$$
where $<>_t$ means averaging over time:
$$
<\cos ^{2}(\omega t)>_{t} \equiv \frac{1}{T}\int^T_{0}dt\cos ^{2}(\omega t) = \frac{1}{2 \pi}\int^{2 \pi}_{0}d\theta \cos ^{2}\theta = \frac{1}{2}
$$
## Linear Superposition Principle
What happens when waves meet?
**Answer:** In normal conditions (vacuum, air, not-too-extreme energies), light behaves linearly
Linear Superposition:
$$
E(x,t) = E_{1}(x,t) + E_{2}(x,t)
$$
Take it for granted.
### Energy Conservation in Superposition
**Naive worry** If two waves with amplitude $A$ add up, we get amplitude doubled and intensity quadrupled - where does the extra energy come from?
**Resolution** 

## Standing Waves
Consider two waves with the same frequency and amplitude, but propagating in the opposite directions: $k_1=-k_2=k$
$$
\psi(x,t) = A\cos(kx-\omega t)+A\cos(kx+\omega t)
$$
$$
\cos \alpha+\cos \beta= 2\cos\frac{\alpha + \beta}{2}\cos\frac{\alpha-\beta}{2}
$$
$$
\Rightarrow \psi(x,t) = 2A \cos(kx)\cos(\omega t)
$$
This is a standing wave:
	No propagation
	Fixed positions of maximum intensity (antinodes): $kx = m\pi \Rightarrow x = 2m\lambda$
	Fixed positions of zero intensity (nodes): $kx=(m + \frac{1}{2})\pi \Rightarrow x = (2m+1)\lambda$
	Energy oscillates between kinetic and potential

## Fourier Transform in Space
Fundamental principle: Every wave can be written as superposition of monochromatic waves:
$$
\psi(x,t) = \frac{1}{\sqrt{ 2 \pi }}\int_{-\infty}^{\infty} \tilde{\psi}(k)e^{i(kx-ckt)} \, dk
$$
where the dispersion relation in vacuum is assumed $\omega(k)=ck$

Fourier transform is the "weight" of each frequency component
$$
\tilde{\psi}(k) = \frac{1}{\sqrt{ 2 \pi }}\int_{-\infty}^{\infty} \psi(x,0) \, dk 
$$

## Gaussian Wave Packets
Gaussian wave packet:
$$
\psi(x,t) = \frac{1}{(\pi a^{2})^{1/4}}e^{-\frac{(x_{0}ct)^{2}}{2a^{2}}}e^{i(k_{0}x-\omega_{0}t)}
$$
Its Fourier transform is also Gaussian:
$$
\tilde{\psi}(k) = \frac{1}{(\pi \kappa^{2})^{\frac{1}{4}}}e^{-\frac{(k-k_{0})^{2}}{2\kappa^{2}}}
$$
where $\kappa=\frac{1}{a}$

Demonstrates uncertainty principle:
	Narrow in space (small $a$) $\leftrightarrow$ Broad in frequency (large $\kappa$)

## More about Gaussians
The Gaussian function $e^{-x^{2}}$ is one of the most ubiquitous functions:
- In statistics, it describes the typical distribution of a large population
- In physics modeling, it is generically used to model "something confined"
- In our course, it was the transverse profile of the laser beam: it decreases rapidly but is infinitely differentiable, contrary to the more brutal option of square profies
- In quantum physics, gaussians are the only wave functions that saturate the Heisenberg Uncertainty principle $\Delta p \Delta t \geq \frac{\hbar}{2}$ 

Normalise Gaussians
Use the formula
$$
\int_{-\infty}^{\infty} e^{-u^{2}} \, du = \sqrt{ \pi } 
$$
To find the normalization factor $A(a)$ of a Gaussian
$$
G(x) = A(a)
$$
