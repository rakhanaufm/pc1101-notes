# Superposing Two Monochromatic Waves in 1D
Prove that
$$
\begin{split}
\psi(x,t) & = A_{1}\cos(k_{1}x - \omega_{1}t + \phi_{1}) + A_{2}\cos(k_{2}x-\omega_{2}t+\phi_{2}) \\
& =(A_{1}+A_{2})\cos(S_{+})\cos(S_{-}) + (A_{2}-A_{1})\sin(S_{+})\sin(S_{-}),
\end{split}
$$
where
$$
S_{\pm}=\frac{1}{2}[(k_{1}\pm k_{2})x-(\omega_{1}\pm \omega_{2})t + (\phi_{1} \pm \phi_{2})]
$$

## Answer
Observe that 
$$
\cos(A)\cos(B)-\sin(A)\sin(B) = \cos(A+B)
$$
and
$$
\cos(A)\cos(B)+\sin(A)\sin(B)=\cos(A-B)
$$
Hence, we can reduce the given function into,
$$
\begin{split}
\psi(x,t) & = A_{1}(\cos(S_{+})\cos(S_{-})-\sin(S_{+})\sin(S_{-})) + A_{2}(\cos(S_{+})\cos(S_{-}) + \sin(S_{+})+\sin(S_{-})) \\
& = A_{1}\cos(S_{+}+S_{-}) + A_{2}\cos(S_{+}-S_{-}) \\
& = A_{1}\cos\left(\frac{1}{2}((2k_{1}+k_{2}-k_{2})x -(2\omega_{1}+\omega_{2}-\omega_{2})t+(2\phi_{1}+\phi_{2}-\phi_{2}))\right) \\
& \space \space\space\space\space+ A_{2}\cos\left(\frac{1}{2}((k_{1}-k_{1}+2k_{2})x-(\omega_{1}-\omega_{1}+2\omega_{2})t+(\phi_{1}-\phi_{1}+2\phi_{2}))\right) \\
& = A_{1}\cos(k_{1}x - \omega_{1}t + \phi_{1}) + A_{2}\cos(k_{2}x-\omega_{2}t+\phi_{2})
\end{split}

$$
Q.E.D.


# Forced Oscillations
Repeat the analysis in class to find and verify the solution to the following forced oscillation:
$$
\ddot{f}(t)+2\beta \dot{f}(t) + \omega_{0}^2f(t) = D_{0}\sin(\omega t)
$$
Compare your result to the classroom solution and comment

## Answer 
The following differential equation has a solution $f(t)$ which has a homogeneous term $f_{h}(t)$ and non homogeneous term $f_{nh}(t)$. We first try to find the homogeneous solution by setting the right hand side to zero:
$$
\ddot{f}(t) + 2 \beta \dot{f}(t) + \omega _{0}^2f(t) = 0
$$
Which has a characteristic equation:
$$
r^2 + 2 \beta r + \omega_{0}^2 = 0
$$
Using the quadratic formula, the roots are:
$$
r = - \beta \pm \sqrt{ \beta^2 -\omega_{0}^2 }
$$
Depending on the discriminant $(\beta^2 - \omega_0^2)$ we have three cases:
- Overdamped: $\beta^2 > \omega_0^2$
- Critically damped: $\beta^2 = \omega_0^2$
- Underdamped: $\beta^2 < \omega_0^2$
For the general solution, we have:
$$
f_{h}(t)= C_{1}e^{-\beta t}e^{i \omega t} + C_{2}e^{- \beta t}e^{-i \omega t}
$$
where the angular frequency $\omega$ is
$$
\omega = \sqrt{\omega_{0}^2 - \beta^2  }
$$
To find the nonhomogeneous solution, we assume a solution of the form:
$$
f_{nh}(t) = A\sin(\omega t) + B\cos(\omega t)
$$
Calculating the first and second derivatives gives:
$$
\dot{f}_{nh}(t) = A \omega \cos(\omega t) -B\omega \sin(\omega t)
$$
$$
\ddot{f}_{nh}(t)=-A\omega^2\sin(\omega t) -B\omega^2\cos(\omega t)
$$
Substituting these into the original equation, we have:
$$
\begin{align}
(-A\omega^2\sin(\omega t) -B\omega^2\cos(\omega t)) &+ 2\beta(A \omega \cos(\omega t) -B\omega \sin(\omega t)) + \omega_{0}^2(A\sin(\omega t) + B\cos(\omega t))  \\
& = D_{0}\sin(\omega t)
\end{align}
$$

Grouping terms:
- Coefficient of $\sin(\omega t)$:
$$
-\omega^2A+\omega_{0}^2A-2\beta \omega B=D_{0}
$$
- Coefficient of $\cos(\omega t)$:
$$
-\omega^2B+\omega_{0}^2B+2\beta \omega A=0
$$
This yields a system of equations:
$$
A(\omega_{0}^{2}-\omega^2)-2\beta \omega B=D_{0}
$$
$$
B(\omega_{0}^2-\omega^2) +2\beta \omega A=0
$$
Solve the system of equations:
From the second equation, we can express $B$:
$$
B = - \frac{2 \beta \omega A}{\omega_{0}^2-\omega^2}
$$
Substituting into the first equation gives:
$$
A(\omega_{0}^2-\omega^2)+\frac{4\beta^2\omega^2 A}{\omega_{0}^2-\omega^2}=D_{0}
$$
This simplifies to:
$$
A\left(\omega_{0}^2-\omega^2+\frac{4\beta^2\omega^2}{\omega_{0}^2-\omega^2}\right) =D_{0}
$$
Solving for $A$ gives:
$$
A = \frac{(\omega_{0}^2-\omega^2)D_{0}}{(\omega_{0}^2-\omega^2)^2+4\beta^2\omega^2}
$$
Substituting into B gives:
$$
B = -\frac{2 \beta \omega D_{0}}{(\omega_{0}^2-\omega^2)^2+4\beta^2\omega^2}
$$

We then combine the two solutions to get the final solution,
$$
f(t) = \frac{(\omega_{0}^2-\omega^2)D_{0}}{(\omega_{0}^2-\omega^2)^2+4\beta^2\omega^2}\sin(\omega t) -\frac{2 \beta \omega D_{0}}{(\omega_{0}^2-\omega^2)^2+4\beta^2\omega^2}\cos(\omega t) + C_{1}e^{-\beta t}e^{i \omega t} + C_{2}e^{- \beta t}e^{-i \omega t}
$$

We obtain a pretty similar solution with the one in class. However, the $(\omega_{0}^{2}-\omega^2)^{2}$ term is flipped in the solution for $\cos(\omega t)$ driving term


# Fourier Transforms
There are few Fourier transforms that can be computed without integration in the complex plane
(a) Redo the Fourier transform of the square pulse with shifted origin of time:
$$
f(t) = \begin{cases}
Ae^{i\omega_{0} t}  & , 0 \leq t \leq a \\ \\
0  &, otherwise 
\end{cases}
$$
Explain the difference of your result and the one obtained in class.

(b) Compute the Fourier transform of the exponential emission
$$
f(t) = \begin{cases} 
0 & , t < 0 \\ 
Ae^{- \gamma t +i\omega_{0}t} & , t \geq 0
\end{cases}
$$
This is the so-called Lorentzian spectrum, with both a real and imaginary part.

(c) Prove that the Fourier transform of Gaussian function is also a Gaussian:
$$
f(t) = Ae^{- \mu t^2}
$$
where $\mu > 0$.

## Answer
(a) 
$$
\begin{align}
\tilde{f}(\omega) & = \frac{1}{\sqrt{2 \pi }}\int_{-\infty}^{\infty}  \, dt f(t)e^{-i \omega t} \\ 
& = \frac{1}{\sqrt{ 2 \pi }}\int^{a}_{0}Ae^{i \omega_{0} t}e^{-i \omega t} \, dt \\
& = \frac{1}{\sqrt{ 2 \pi }}\int^a_{0}Ae^{(i \omega_{0}-i\omega)t} \, dt \\
& = \frac{1}{\sqrt{ 2 \pi }(i \omega_{0} -i\omega)}\left(Ae^{(i \omega_{0} - i \omega)a}-A\right) \\
& = \frac{A}{\sqrt{ 2\pi }i(\omega-\omega_{0})}e^{-(i(\omega-\omega_{0})a)/2}\left(e^{i(\omega-\omega_{0})a/2} - e^{-i(\omega-\omega_{0})a/2}\right) \\
&= \frac{A}{\sqrt{ 2\pi }i(\omega-\omega_{0})}e^{-i(\omega-\omega_{0})a/2}\left(2i\sin\left( \frac{(\omega-\omega_{0})a}{2} \right)\right) \\
&= \frac{A}{\sqrt{ 2\pi }i(\omega-\omega_{0})}e^{-i(\omega-\omega_{0})/2}2i \frac{(\omega-\omega_{0})a}{2} \frac{\sin\left( \frac{(\omega-\omega_{0})a}{2} \right)}{\frac{(\omega-\omega_{0})a}{2}} \\
&= \frac{Aa}{\sqrt{ 2\pi }}e^{-i(\omega-\omega_{0})a/2} \text{sinc}\left( \frac{(\omega-\omega_{0})a}{2} \right)
\end{align}

$$
as for the difference with the result obtained in class, is the phase factor of $e^{-i(\omega-\omega_{0})a/2}$ which reflects the time shifting property of the Fourier Transform.
(b)
$$
\begin{align}
\tilde{f}(\omega) &= \frac{1}{\sqrt{ 2 \pi }}\int_{-\infty}^{\infty} f(t)e^{-i \omega t} \, dt \\
& = \frac{1}{\sqrt{ 2 \pi }}\int^{\infty}_{0}Ae^{- \gamma t + i \omega_{0} t - i \omega t} dt \\
& = \frac{1}{2 \pi} \int^\infty_{0}Ae^{(-\gamma+i \omega_{0} - i \omega)t} \, dt \\
& = \frac{1}{\sqrt{ 2 \pi } (- \gamma + i \omega_{0}- i \omega)}\left(0 - A\right) \\
& = A\frac{1}{\sqrt{ 2 \pi}( \gamma -i(\omega_{0}-\omega)) } \\
& = A\frac{1}{\sqrt{ 2 \pi} (\gamma^2 + (\omega-\omega_{0})^{2})}\left( \gamma - i(\omega-\omega_{0})\right)
\end{align}

$$
which indeed has a real and imaginary component.
(c) 
$$
\begin{align}
\tilde{f}(\omega) & = \frac{1}{\sqrt{ 2 \pi }}\int_{-\infty}^{\infty} Ae^{- \mu t^2 - i \omega t} \, dt \\
& = \frac{1}{\sqrt{ 2 \pi }} \int_{-\infty}^{\infty} Ae^{-\mu\left( t^2 + \frac{i \omega}{\mu} \right)} \, dt  \\
& = \frac{1}{\sqrt{ 2 \pi }}\int_{-\infty}^{\infty} Ae^{-\mu\left(\left( t + \frac{i \omega}{2 \mu} \right)^2 - \left( \frac{i \omega}{2 \mu} \right)^2\right)} \, dt  \\
& = \frac{Ae^{\mu\left( \frac{i \omega}{2 \mu} \right)^2}}{\sqrt{ 2 \pi }}\sqrt{ \frac{\pi}{\mu} } \\
& = A \sqrt{ \frac{1}{2 \mu } }e^{-\frac{\omega^2}{4 \mu}}
\end{align}
$$
which is also a Gaussian.

