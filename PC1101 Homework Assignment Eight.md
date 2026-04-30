Muhammad Rakha Naufal Maulana A0330820U
# 1. More On Planck's Blackbody Formula
a)
To maximize $\epsilon_{Planck}(\lambda)$, we have the condition
$$
\frac{d\epsilon_{Planck}}{d\lambda} = 0 
$$
Set $\frac{d\epsilon}{d\lambda} = 0$. Let $u = \frac{hc}{\lambda k_{B}T}$, so $\lambda = \frac{hc}{uk_{B}T}$
The condition $\frac{d\epsilon}{d\lambda} = 0$ becomes (after algebra):
$$
\frac{d}{d\lambda} [\lambda^{-5}(e^{hc/\lambda k_{B}T}-1)^{-1}] = 0
$$
Computing the derivative and setting it to zero:
$$
-5 \lambda^{-6}(e^u-1)^{-1} + \lambda^{-5} \cdot \frac{e^u}{(e^u-1)^{2}} \cdot \frac{hc}{\lambda^{2}k_{B}T} = 0
$$
Multiply through by $\lambda^6(e^u-1)$:
$$
-5(e^u-1)+ue^u = 0
$$
This gives the transcendental equation:
$$
(5-u)e^u = 5
$$
This must be solved numerically. Using a calculator, we can iterate and get $u \approx 4.96511$
Then $\lambda_{peak}T = \frac{hc}{uk_{B}}$:
$$
\lambda_{peak}T = \frac{(6.626 \times 10^{-34})(3 \times 10^8)}{(4.96511)(1.381 \times 10^{-23})} = \frac{1.988 \times 10^{-25}}{6.857 \times 10^{-23}} \approx 2.898
$$
b)
The total intensity must be the same whether integrated over $\lambda$ or $\omega$:
$$
I = \int^{\infty}_{0}d\lambda \epsilon(\lambda) = \int^{\infty}_{0}d\omega\epsilon(\omega)
$$
To solve this, we use the substitution $\omega = \frac{2\pi c}{\lambda}$, so $\lambda = \frac{2\pi c}{\omega}$ and $|\frac{d\lambda}{d\omega}| = \frac{2\pi c}{\omega^{2}}$
Substituting into $\epsilon(\lambda)$:
$$
\epsilon(\omega)d\omega = \epsilon(\lambda) | \frac{d\lambda}{d\omega}| d\omega = \frac{2\pi hc^{2}}{\left( \frac{2\pi c}{\omega} \right)^5} \cdot \frac{1}{e^{\hbar \omega/k_{B}T}-1} \cdot \frac{2\pi c}{\omega^{2}}d\omega
$$
The $\lambda^5$ term becomes $\frac{(2\pi c)^5}{\omega^5}$. Substituting $h = 2\pi \hbar$:
$$
\epsilon(\omega) = \frac{2\pi \cdot 2 \pi \hbar \cdot c^{2} \cdot \omega^5}{(2\pi c)^5} \cdot \frac{1}{e^{\hbar \omega/k_{B}T}-1} = \frac{\hbar \omega^{3}}{(2\pi c)^{2}} \cdot \frac{1}{e^{\hbar \omega/k_{B}T}-1}
$$
$$
\epsilon_{Planck}(\omega) = \frac{\hbar \omega^{3}}{(2\pi c)^{2}} \cdot \frac{1}{e^{\hbar \omega/k_{B}T}-1}
$$
c)
To solve the integral we use the substitution,
$$
u = \frac{\hbar\omega}{k_{B}T}
$$
rewriting the integral,
$$
I = \int^{\infty}_{0} \frac{\hbar}{(2\pi c)^{2}} \left( \frac{uk_{B}T}{\hbar} \right)^{3} \frac{1}{e^u-1} \frac{k_{B}T}{\hbar} du= \int^{\infty}_{0} \frac{(k_{B}T)^4}{(2\pi c)^{2} \hbar^{3}} \frac{u^{3}}{e^u-1} = \frac{(k_{B}T)^{4}}{(2\pi c)^{2} \hbar^{3}} \frac{\pi^4}{15} = \sigma T^4
$$
$$
\sigma = \frac{(k_{B}\pi)^4}{15 (2\pi c)^{2} \hbar^{3} } = \frac{2\pi^5k_{B}^4}{15h^{3}c^{2}}
$$

# 2. The Uncertainty Principle with Gaussian Wave Packets
a)
Since $|\psi|^{2} = (2\pi \sigma^{2})^{-1/2}e^{-x^{2}/2\sigma^{2}}$ is a Gaussian centered at zero:
$$
\langle x \rangle = 0
$$
$$
\langle x^{2} \rangle  = \frac{1}{\sqrt{ 2\pi \sigma^{2} }} \int_{-\infty}^{\infty} x^{2}e^{-x^{2}/2\sigma^{2}} \, d = \sigma^{2}
$$
using the standard Gaussian moment $\int x^{2}e^{-x^{2}/2\sigma^{2}}dx = \sqrt{ 2\pi }\sigma^{3}$
$$
\Delta x = \sigma
$$
b)
$$
\tilde{\psi}(k) = \frac{1}{\sqrt{ 2\pi }} \int_{-\infty}^{\infty} \psi(x,0)e^{-ikx} \, dx 
$$
Substituting $\psi(x,0)$,
$$
\tilde{\psi}(k) = \frac{1}{\sqrt{ 2\pi }} \int_{-\infty}^{\infty} \frac{1}{(2\pi \sigma^{2})^{1/4}}e^{-x^{2}/4\sigma^{2}}e^{ik_{0}x}e^{-ikx} \, dx 
$$
we can take out the normalization factor outside the integral
$$
\tilde{\psi}(k) = \frac{1}{\sqrt{ 2\pi }} \frac{1}{(2\pi \sigma^{2})^{1/4}} \int_{-\infty}^{\infty} e^{-x^{2}/4\sigma^{2} +i(k_{0}-k)} \, dx 
$$
Now we complete the square in the exponent: $-\frac{x^{2}}{4\sigma^{2}} - i(k-k_{0})x = -\frac{1}{4\sigma^{2}}[x + 2i\sigma^{2}(k-k_{0})]^{2} - \sigma^{2}(k-k_{0})^{2}$.
The Gaussian integral gives $\int e^{-(x + const)^{2}/4\sigma^{2}}dx = 2\sigma \sqrt{ \pi }$:
$$
\tilde{\psi}(k) = \frac{2\sigma \sqrt{ \pi }}{(2\pi \sigma^{2})^{1/4}\sqrt{ 2\pi }}e^{-\sigma^{2}(k-k_{0})^{2}} = \left( \frac{2\sigma^{2}}{\pi} \right)^{1/4} e^{-\sigma^{2}(k-k_{0})^{2}}
$$
$$
\tilde{\psi}(k) = \left( \frac{2\sigma^{2}}{\pi} \right)^{1/4} \exp[-\sigma^{2}(k-k_{0})^{2}]
$$
This is itself a Gaussian in $k$-space centered on $k_{0}$, with standard deviation $\frac{1}{2\sigma}$.
c)
$|\tilde{\psi}(k)|^{2} = \left( \frac{2\sigma^{2}}{\pi} \right)^{1/2} e^{-2\sigma^{2}(k-k_{0})^{2}}$ is a Gaussian in $k$ centered at $k_{0}$ with variance $\frac{1}{4\sigma^{2}}$
$$
\langle k \rangle = k_{0}, \langle k^{2} \rangle -\langle k \rangle ^{2} = \frac{1}{4\sigma^{2}}
$$
$$
\Delta k = \frac{1}{2\sigma}, \Delta p = \hbar\Delta k = \frac{\hbar}{2\sigma}
$$
d)
$$
\Delta x \cdot \Delta p = \sigma \cdot \frac{\hbar}{2\sigma} = \frac{\hbar}{2}
$$
$$
\Delta x\Delta p = \frac{\hbar}{2} \geq \frac{\hbar}{2}
$$
The Gaussian saturates the Heisenberg bound, it is the minimum uncertainty state. No other normalised wave packet achieves a smaller product of $\Delta x\Delta p$.