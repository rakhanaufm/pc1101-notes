# Wave Optics
## Oscillations
### Simple Harmonic Motion
$$
\ddot{f}(t) = -\omega^2f(t)
$$
It is a constant coefficient 2nd-order ordinary differential equation
- It can be solved by an exponential function
Where $\omega$ is called angular frequency, $rad/s$

Assume that the solution is an exponential solution:
$$
f(t) = ke^{\mu t}
$$
Where $k$ and $\mu$ are two constants
If $f(t)$ is a solution, then $2f(t)$ must be a solution too
$\Rightarrow k$ is arbitrary
Plug into the equation
$$
\dot{f}= k \mu e^{m t}, \ddot{f} = k \mu^2 e^{\mu t} = \mu^2f = - \omega^2 f
$$
we get $\mu^2$ . Thus $\mu$ = $\pm i \omega$
$\Rightarrow$ A general solution: $f_1(t) = C_1e^{i \omega t} + C_2e^{-i \omega t}$ 

### Damped Oscillation
$$
\ddot{f}(t) + 2\beta \dot{f}(t) + \omega_{0}^2f(t) = 0
$$
It is  a constant coefficient 2nd-order ordinary differential equation
Solution:
$$
f(t) = C_{1}e^{-\beta t}e^{i\omega t}+C_{2}e^{-\beta t}e^{-i\omega t}
$$
Where the angular frequency is
$$
 \omega \equiv \sqrt{ \omega_{0}^2-\beta^2 }
$$
#### Under-damped: $\beta < \omega_0$
- The solution can be rewritten as $f(t) = Ae^{-\beta t} \cos(\omega t + \phi)$
- $Ae^{- \beta t}$ can be considered as a diminishing amplitude
#### Critical Damping: $\beta = \omega_0$
- $\omega = 0$ , another linearly independent solution is needed.
- $f(t) = C_1e^{-\beta t} + C_2te^{-\beta t}$ 
#### Over-damped: $\beta > \omega_0$
- No oscillation:
$$
f(t) = C_{1}e^{-(\beta-\mu)t}+C_{2}e^{-(\beta+\mu)t}
$$
- Where $\mu \equiv i \omega = \sqrt{\beta^2 - \omega_0^2}$ is a real parameter

### Forced Oscillation
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

### Fourier Transform
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
## Wave Optics
### Interference
$S_{1}$ and $S_2$ are two coherent wave sources
Consructive interference occurs when the path difference is an integral number of wavelengths
Destructive interference occurs when the path difference is a half-integral number of wavelengths
Consider two oscillations with a phase difference $\phi$,
$$
E_{1}(t)=E_{0}\cos(\omega t), E_{2}(t) = E_{0}\cos(\omega t+\phi)
$$
The resultant amplitude satisfies
$$
\begin{align}
E(t) &= E_{1}(t) + E_{2}(t) = E_{0}[\cos(\omega t)+\cos(\omega t+\phi)] \\
&= 2E_{0}\cos \frac{\omega t+\omega t+\phi}{2} \cos \frac{\omega t-(\omega t + \phi)}{2}  \\
&= 2E_{0}\cos\left[ \omega t + \frac{\phi}{2} \right] \cos \frac{\phi}{2}
\end{align}
$$
Averaging in time of the amplitude square:
$$
\langle E(t)^{2} \rangle = 4E_{0}^{2} \left\langle  \cos ^{2}\left( \omega t + \frac{\phi}{2} \right)  \right\rangle \cos ^{2} \frac{\phi}{2} = 2E_{0}^{2} \cos ^{2} \frac{\phi}{2}
$$
In terms of the incoming light,
$$
\langle E_{1}^{2}(t) \rangle = \langle E_{0}^{2}\cos ^{2} \omega t \rangle = E_{0}^{2} \langle \cos ^{2}\omega t \rangle = \frac{1}{2}E_{0}^{2}
$$
$$
\langle E^{2}(t) \rangle  = 4 \langle E_{1}^{2}(t) \rangle \cos ^{2} \frac{\phi}{2}
$$
Thus, the intensity of double slit interference is
$$
I = 4 I_{0} \cos ^{2} \frac{\phi}{2}
$$
where $\phi = \frac{2\pi}{\lambda}d\sin \theta=kd\sin \theta$
### Diffraction
#### Spherical Waves
Second common wave type
$$
\frac{A}{r(\mathbf{x})}\cos[kr(\mathbf{x})-\omega t+\phi]
$$
Where: $r(\textbf{x}) \equiv |\mathbf{x}-\mathbf{x}_{0}|= \sqrt{ (x-x_{0})^{2}+(y-y_{0})^{2}+(z-z_{0})^{2} }$
Wavefronts: Spheres centered at source $\textbf{x}_0$
Amplitude decay: $1/r$ from energy conservation
Energy conservation: Same energy spreads over larger sphere
#### Fraunhofer Diffraction
By Huygens' principle, each point in slit acts as source:
$$
E(\mathbf{x},t) = \int^{\frac{a}{2}}_{-\frac{a}{2}} dy_{0} \frac{A}{r}\cos(kr-\omega t)
$$
Far field approximations ($R \gg a$):
Amplitude factor:
$$
\frac{1}{r} \approx \frac{1}{R}
$$
Phase factor:
$$
r \approx R-y_{0}\sin \theta
$$
I'm taking PC3247 yay so I will learn this 
$$
E(\mathbf{x},t) \approx \frac{A}{R} \int^{\frac{a}{2}}_{-\frac{a}{2}}dy_{0}\cos(k(R-y_{0}\sin \theta)-\omega t)
$$
$$
=\frac{A}{R} \frac{1}{-k\sin \theta} \sin[kR- \omega t -k y_{0}\sin \theta] |^{a/2}_{-\frac{a}{2}}
$$
$$
=\frac{A}{R} \frac{1}{-k\sin \theta} \left( -2\cos(kR-\omega t)\sin \frac{ka\sin \theta}{2} \right)
$$
$$
= \frac{A}{R} \frac{1}{k\sin \theta} 2\cos (kR- \omega t) \sin \frac{ka\sin \theta}{2}
$$
$$
= \frac{aA}{R} \cos(kR-\omega t) \text{sinc} \frac{ka\sin \theta}{2}
$$

#### Diffraction Result
Final result:
$$
E(\mathbf{x},t) = \frac{aA}{R} \cos(kR- \omega t) \text{sinc} \frac{ka\sin \theta}{2}
$$
Where: $\text{sinc}(\beta) \equiv \frac{\sin \beta}{\beta}$
Key feature: Amplitude depends on direction through $\text{sinc} \frac{ka\sin \theta}{2}$

$$
\Rightarrow I(\theta) \propto \text{sinc}^{2}\left( \frac{ka}{2}\sin \theta \right)
$$
### Polarisation
Electric field is a vector
Light is a transverse wave: $\textbf{E}$ perpendicular to propagation direction
Polarisation: Direction of electric field oscillation
Define orthogonal unit vectors in transverse plane:
	$\hat{\textbf{e}}_H$ (horizontal) and $\hat{\textbf{e}}_V$ (vertical)
Such that $\hat{\mathbf{e}}_{H} \times \hat{\mathbf{e}}_{V}= \hat{\mathbf{e}}_{k}$
#### Linear Polarisation
Electric field oscillates along fixed direction:
$$
\mathbf{E}(\mathbf{x},t)=E_{0}\cos(k\mathbf{z}-\omega t+\phi)
$$
Where: $\hat{\mathbf{e}}_{\theta} \equiv \cos \theta \hat{\mathbf{e}}_{H}+\sin \theta \hat{\mathbf{e}}_{V}$
Field oscillates along direction $\theta$
Note: $\theta'= \theta + \pi$ gives same polarisation
Most common type in everyday applications

#### Circular Polarisation
Electric field **rotates** around propagation axis
$$
\mathbf{E}(\mathbf{x},t) = \frac{E_{0}}{\sqrt{ 2 }}[\cos (k\mathbf{z}-\omega t+\phi)\hat{\mathbf{e}}_{H} \pm \sin (k\mathbf{z}-\omega t+\phi) \hat{\mathbf{e}}_{V}]
$$
Right-handed: - sign
	(counterclockwise from receiver view)
Left-handed: + sign
	(clockwise from receiver view)
Factor $1/\sqrt{ 2 }$  ensures proper normalisation

#### Elliptical Polarisation
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
### Amplitude & Intensity
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
### Plane Wave
A monochromatic plane wave is given by
$$
A\cos(\mathbf{k}\cdot \mathbf{x} - \omega t + \phi)
$$
Wave vector: $\textbf{k}=k\hat{\mathbf{e}}_k$ carries magnitude and direction
Propagates in direction of $\textbf{k}$
Dispersion relation: $\omega = c|\textbf{k}|$ 
Wavefronts: Planes perpendicular to $\hat{\mathbf{e}}_k$
### Gaussian Wave Packet
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
Normalise Gaussians
Use the formula
$$
\int_{-\infty}^{\infty} e^{-u^{2}} \, du = \sqrt{ \pi } 
$$
To find the normalization factor $A(a)$ of a Gaussian
$$
G(x) = A(a)
$$

# Relativity
## Special Relativity
### Principle: All inertial frames are equivalent
Note: the transverse distances are the same in both inertial frames.
Observe that
$$
-(c\Delta t)^{2} + (\Delta x)^{2} = -4D^{2} = -(c\Delta t_{0})^{2}
$$
Or
$$
-(cdt)^{2} + (dx)^{2} + (dy)^{2} + (dz)^{2} = -(cdt_{0})^{2} + (dx_{0})^{2}+(dy_{0})^{2} + (dz_{0})^{2}
$$
$$
ds^{2}=ds_{0}^{2}
$$
An invariance between these two inertial frames

### Lorentz Transformation
Lorentz boost by $\theta$:
	$ct' = ct\cosh \theta -x\sinh \theta$
	$x'=-ct\sinh \theta + x\cosh \theta$
Lorentz invariance
$$
ds'^{2}=ds^{2}
$$
Velocity of $S'$ relative to $S$:
$$
v = c\tanh \theta
$$

### Length contraction & Time dilation
The rate at which time flows depends on how fast the observer moves!
$$
\Delta t = \frac{\Delta t_{0}}{\sqrt{ 1-\left( \frac{v}{c} \right)^{2} }} = \gamma t_{0}
$$
Note: this is not just the subjective perception of time, but the objective measurable length of time!

Consider a rod whose length is $L_{\star}$ when measured in its own rest frame.
$$
x' = \gamma(x-vt), t' = \gamma\left( t- \frac{vx}{c^{2}} \right)
$$
$$
\Delta x' = \gamma(\Delta x -v\Delta t), \Delta t' = \gamma\left( \Delta t - \frac{v}{c^{2}}\Delta x \right)
$$
$$
\Delta t'=0, \Delta x' = L, \Delta t \neq 0 , \Delta x = L_{\star}
$$
$$
\begin{cases}
L &= \gamma(L_{\star}-v \Delta t) \\
0 &= \gamma\left( \Delta t - \frac{v}{c^{2}}L_{\star} \right) \Rightarrow \Delta t = \frac{v}{c^{2}}L_{\star} 
\end{cases}
$$
$$
L = \frac{L_{\star}}{\gamma}
$$
### Twin Paradox
Astronaut Alice takes a space trip at a speed of $\beta = 0.65$ to a space station located 3.25 light-years from Earth and back starting on the 20th birthday while her twin brother Bob stays at home on Earth.
The round trip distance is 6.5 light-years, so from Bob's point of view on Earth, Alice's trip takes
$$
\frac{6.50}{0.65} = 10 \space \text{years}
$$
So when Alice returns, Bob is 20 + 10 = 30 years old
#### Length Contraction
The gamma parameter for Alice is
$$
\gamma = \frac{1}{\sqrt{ 1- 0.65^{2} }} = 1.315
$$
From Alice's point of view, she travels a length contracted distance
$$
\frac{6.5}{1.315} = 4.942
$$
From Alice's point of view, the trip takes
$$
\frac{4.942}{0.65} = 7.6 \space \text{years}
$$
When she returns, Alice is 20 + 7.6 = 27.6 years old
#### The Paradox
Now let's look at Bob from Alice's point of view
Whe seems to be sitting still and Bob is moving with speed $\beta=0.65$
Alice ages 7.6 years during her trip, but Bob was moving with $\beta = 0.65$ $(\gamma \approx 1.316)$ so his clock was running more slowly and he should have aged
$$
\frac{7.6}{1.316} = 5.8 \space \text{years}
$$
So when Alice returned to Earth, she would be 27.6 years old and Bob would be 25.8 years old
Both twins can't be younger than the other!
Which of these two views is right?
#### Resolution of the Twin Paradox
The resolution of the twin paradox comes when we realize that Bob remains in an inertial frame on Earth while Alice lives in two different inertial frames during her trip
	An outbound leg where she moves away from Earth and towards the space station
	An inbound leg where she moves back from the space station towards Earth
	The symmetry between the twins is broken!
We can analyze the path of the two twins by counting "Happy Birthday" signals they received from each other

### Addition of velocities
Lorentz transformation
$$
\begin{cases}
t = \gamma\left( t' - \frac{vx'}{c^{2}} \right) \\
x = \gamma(x' - vt') 
\end{cases}
$$
Differentiating, we get
$$
\begin{cases}
dt = \gamma\left( dt' - \frac{vdx'}{c^{2}} \right) \\
dx = \gamma(dx' - vdt')
\end{cases}
$$
taking $\frac{dx}{dt}$, we get
$$
\frac{dx}{dt} = \frac{\left( dt' - \frac{vdx'}{c^{2}} \right)}{dx' - vdt'} = \frac{\left( 1 - \frac{vdx'}{dt'c^{2}} \right)}{\frac{dx'}{dt'} - v}
$$
Rearranging for $\frac{dx'}{dt'}$ and using $v_{1+2} = \frac{dx'}{dt'}$ and $u = \frac{dx}{dt}$, we get
$$
v_{1+2} = \frac{u + v}{1 + \frac{uv}{c^{2}}}
$$
### Energy-momentum relation
#### Momentum and Energy (1)
Start with the results for momentum and energy and square:
$$
\vec{p} = \gamma m \vec{v} \Rightarrow p^{2} = \gamma^{2}m^{2}v^{2}
$$
$$
E = \gamma mc^{2} \Rightarrow E^{2} = \gamma^{2} m^{2}c^4
$$
Square of the gamma-factor:
$$
\gamma^{2} = \frac{1}{1 - \beta^{2}} = \frac{1}{1 - \frac{v^{2}}{c^{2}}} = \frac{c^{2}}{c^{2} - v^{2}}
$$
Express $E^{2}$ as a function of $p^{2}$:
$$
E^{2} = \frac{c^{2}}{c^{2} - v^{2}} m^{2}c^4 = m^{2}c^4 + \frac{v^{2}}{c^{2}-v^{2}}m^{2}c^4
$$
$$
m^{2}c^4 + \frac{c^{2}}{c^{2}-v^{2}}m^{2}v^{2}c^{2} = m^{2}c^4 + \gamma^{2}m^{2}v^{2}c^{2}
$$
$$
E^{2} = m^{2}c^4 + p^{2}c^{2}
$$
#### Momentum and Energy (2)
Finally we take the square root
$$
E = \sqrt{ p^{2}c^{2} + m^{2}c^4 }
$$
Special case with no motion:
$$
E = mc^{2}
$$
Negative root: antimatter (Dirac)
$$
E = - \sqrt{ p^{2}c^{2} + m^{2}c^4 }
$$
Case of zero mass (photons):
$$
E = pc
$$
#### Speed, Energy, and Momentum
Divide momentum by energy
$$
\frac{p}{E} = \frac{\gamma m v}{\gamma mc^{2}} = \frac{v}{c^{2}} \Rightarrow \frac{pc^{2}}{E}
$$
This gives us an additional energy-momentum relationship:
$$
\beta = \frac{pc}{E} \Rightarrow p = \frac{\beta E}{c} or E = \frac{pc}{\beta}
$$
### Doppler effect & Relativistic beaming
Lorentz boost:
$$
\omega' = \gamma(\omega + vk^x), \space k^{x'} = \gamma\left( k^x + \frac{v\omega}{c^{2}} \right)
$$
$$
|\vec{k}| = \frac{\omega}{c}, \space k^x = |\vec{k}|\cos \alpha
$$
with $\alpha$ the angle with the x axis
$$
\Rightarrow
\begin{cases}
\omega' = \gamma\left( \omega + \frac{v\omega}{c}\cos \alpha \right) = \gamma\left( 1 + \frac{v}{c}\cos \alpha \right)\omega \dots(1)\\
\frac{\omega'}{c}\cos \alpha' = \gamma\left( \frac{\omega}{c}\cos \alpha + \frac{v\omega}{c^{2}} \right) \to \omega'\cos \alpha' = \gamma\left( \cos \alpha + \frac{v}{c} \right)\omega \dots(2)
\end{cases}
$$
Cancel $\cos \alpha$:
$$
(1) - \frac{v}{c}(2) \Rightarrow \omega' - \frac{v}{c}\omega'\cos \alpha' = \gamma \omega\left( 1 - \frac{v^{2}}{c^{2}} \right) = \omega \sqrt{ 1 - \frac{v^{2}}{c^{2}} }
$$
Doppler shift:
$$
\Rightarrow \omega' = \frac{\sqrt{ 1 - \frac{v^{2}}{c^{2}} }}{1 - \frac{v}{c}\cos \alpha'}\omega
$$

#### Relativistic Beaming
A uniformly radiating body moving toward you is brighter than if it is moving away
$$
\frac{2}{1} \Rightarrow \cos \alpha' = \frac{ \frac{v}{c} +\cos \alpha}{1 + \frac{v}{c}\cos \alpha}
$$
#### Forward and Backward Emissions
Forward emission, $-\frac{\pi}{2} \leq \alpha \leq \frac{\pi}{2}$,
$$
\frac{v}{c} \leq \frac{v}{c} + \frac{\left( 1-\frac{v^{2}}{c^{2}} \right)\cos \alpha}{1 + \frac{v}{c}\cos \alpha} = \cos \alpha' = \frac{\cos \alpha + \frac{v}{c} }{1 + \frac{v}{c}\cos \alpha} = 1 - \frac{(c-v)(1-\cos \alpha)}{c+v\cos \alpha} \leq 1
$$
Backward emission, $-\pi \leq \alpha \leq -\frac{\pi}{2}$,
$$
-1 \leq -1 + \frac{(c-v)(1+\cos \alpha)}{c+v\cos \alpha} 
$$
## General Relativity
### Principle: All frames are equivalent
To simplify the analysis:
$$
\frac{V}{c}, \space \frac{gh}{c^{2}}\space \text{important}
$$
$$
\left( \frac{V}{c} \right)^{2}, \space \left( \frac{gh}{c^{2}} \right)^{2} \space \text{negligible}
$$
Newtonian mechanics can be used!
Consider the emission of two successive light pulses by Alice and their reception by Bob
Suppose that $t=0$ is the time the first pulse is emitted, $t_{1}$ is the time it is received, $\Delta \tau_{A}$ is the time the second pulse is emitted, and $t_{1} + \Delta \tau_{B}$ is the time the second pulse is received
$$
z_{A}(t) = h + \frac{1}{2}gt^{2}
$$
$$
z_{B}(t) = \frac{1}{2}gt^{2}
$$
$$
\Rightarrow \Delta \tau_{B} \approx \left( 1- \frac{gh}{c^{2}} \right)
$$
Signal 1
$$
A_{1}(t=0, z = h) \to B_{1}\left( t_{1}, \frac{1}{2}gt_{1}^{2} \right)
$$
Signal 2
$$
A_{2}\left( \Delta \tau_{A}, h + \frac{1}{2}g\Delta \tau_{A}^{2} \right) \to B_{2}\left( t_{1} + \Delta \tau_{B}, \frac{1}{2}g(t_{1} + \Delta \tau_{B})^{2} \right)
$$
Signal 1
$$
ct_{1} = h - \frac{1}{2}gt_{1}^{2} \Rightarrow \frac{1}{2}gt_{1}^{2} + ct_{1} - h = 0
$$
$$
\Rightarrow t_{1} = \frac{-c \pm \sqrt{ c^{2} +2gh }}{g} \Rightarrow t_{1} = \frac{c}{g}\left[ \sqrt{ 1 + \frac{2gh}{c^{2}} }-1 \right]
$$
Signal 2
$$
c(t_{1} + \Delta \tau_{B} - \Delta \tau_{A}) = h + \frac{1}{2}g\Delta \tau_{A}^{2} - \frac{1}{2} g (t_{1} + \Delta \tau_{B}^{2})
$$
$$
\Rightarrow \frac{1}{2}g (t_{1} + \Delta \tau_{B}^{2}) + c(t_{1} + \Delta \tau_{B}) - \left( h + \frac{1}{2}g \Delta \tau_{A}^{2} + c\Delta \tau_{A} \right) = 0
$$
$$
t_{1} + \Delta \tau_{B} = \frac{ -c \pm \sqrt{ c^{2} + 2g\left( h + \frac{1}{2}g\Delta \tau_{A}^{2} + c\Delta \tau_{A} \right) } }{g}
$$
$$
\Delta \tau_{B} = t_{1} + \Delta \tau_{B} - t_{1} = \frac{c}{g} \left[ \sqrt{ 1 + \frac{2gh}{c^{2}}\left( 1 + \frac{c\Delta \tau_{A}}{h} + \frac{1}{2} \frac{g\Delta \tau_{A}^{2}}{h} \right) } - \sqrt{ 1 + \frac{2gh}{c^{2}} } \right]
$$
$$
\sqrt{ 1+x } \approx 1 + \frac{1}{2}x - \frac{1}{8}x^{2}
$$
$$
\approx \frac{c}{g} \left[ 1+ \frac{gh}{c^{2}}\left( 1 + \frac{c}{h}\Delta \tau_{A} + \frac{1}{2} \frac{g\Delta \tau_{A}^{2}}{h} \right) - \frac{1}{8} \left( \frac{2gh}{c^{2}} \right)^{2} \left( 1 + \frac{c\Delta \tau_{A}}{h} + \dots \right)^{2} - \left( 1 + \frac{gh}{c} - \frac{1}{8} \left( \frac{2gh}{c^{2}} \right)^{2} \right) \right]
$$
$$
= \frac{c}{g} \left[ \frac{g\Delta \tau_{A}}{c} + \frac{1}{2} \frac{g^{2}\Delta \tau_{A}^{2}}{c^{2}} + \frac{1}{2} \frac{g^{2}h^{2}}{c^4}- \frac{1}{2} \frac{g^{2}h^{2}}{c^4} \left(  1 + \frac{c^{2}\Delta \tau_{A}^{2}}{h^{2}} + \frac{1}{4} \frac{g^{2}\Delta \tau_{A}^4}{h^{2}} + \frac{2c\Delta \tau_{A}}{h}  + \frac{cg\Delta \tau_{A}^3}{h^3} \right) \right]
$$
$$
\Delta \tau_{B} \approx \frac{c}{g} \left[  \frac{g\Delta \tau_{A}}{c} - \frac{g^{2}h^{2}}{2c^4} \left(  \frac{g^{2}\Delta \tau_{A}^4}{4h^{2}} + 2 \frac{c\Delta \tau_{A}}{h}  + \frac{gc\Delta \tau_{A}^3}{h^3} \right) \right]
$$
$$
= \Delta \tau_{A} - \frac{1}{8} \frac{g^3}{c^3}\Delta \tau_{A}^4 - \frac{gh}{c^{2}}\Delta \tau_{A} - \frac{g^{2}h}{2c^{3}}\Delta \tau_{A}^{2} - \frac{1}{2} \frac{g^{2}}{c^{2}h}\Delta \tau_{A}^4
$$
$$
= \Delta \tau_{A} \left[ 1 - \frac{1}{8} \left( \frac{g\Delta \tau_{A}}{c} \right)^{3} - \frac{gh}{c^{2}} - \frac{1}{2}\left( \frac{g\Delta \tau_{A}}{c} \right)^{2} \right]
$$
$$
\approx \Delta \tau_{A}\left( 1 - \frac{gh}{c^{2}} \right)
$$
$gh$: Gravitational Potential
### Gravitational redshift
The crests of a light wave of definite frequency can be thought of as a series of signals emitted at a rate that is the frequency of the wave.
$$
\omega_{\infty} = \left( 1 - \frac{GM}{Rc^{2}} \right)\omega_{\star}
$$
Twin paradox tested (1971)
$$
\Delta \tau = \frac{1}{c^{2}} \int dt \{gh(t) - \frac{1}{2}V_{g}(t)\left[ V_{g}(t) + 2V_{\otimes} \right]\}
$$
### Black holes
Schwardzschild Radius
$$
R_{s} = \frac{2GM}{c^{2}}
$$
What happens if the gravitational lensing is so strong that light cannot escape the lens.
# Quantum Mechanics
## Light as Particles
Blackbody radiation
### Photoelectric effect
Light may kick electrons out of metals.
Higher intensity, more electrons.
However, blue light striking cesium causes the cesium to emit electrons. Red light does not, regardless of light intensity.
Light comes in photons.
To emit an electron, the cesium atom must absorb a single photon whose energy exceeds the ionization energy of the outermost electron in cesium.
A blue photon has enough energy; a red photon does not.
Each photon carries energy:
$$
E = hf = \hbar \omega
$$

### Energy-momentum conservation
Compton Scattering
Photon carries momentum too.
$$
\mathbf{p}=\hbar \mathbf{k}
$$
Momentum conservation
$$
\mathbf{p}=\mathbf{p}' + \mathbf{P}_{e}
$$
Energy conservation
$$
h \frac{c}{\lambda} + m_{e}c^{2} = h \frac{c}{\lambda'} + E_{e}
$$
where $E_{e}^{2} = m_{e}^{2}+P_{e}^{2}c^{2}$
Wavelength shift
$$
\Delta \lambda = \frac{h}{m_{e}c}(1-\cos \phi)
$$
## Principles of QM
### Wavefunctions
Wavefunctions contain all quantum information about a system's state and evolution
Wavefunctions can be complex-valued and with multiple components
Governed by the Schrodinger equation in non-relativistic quantum mechanics
Not directly measurable - serve as mathematical framework for calculating observable quantities
Upon measurement, wavefunctions collapse to definite states
Measurements yield discrete, quantized values
The system remains in the measured state post-collapse
Wave-particle duality: while the wavefunction evolves continuously, observations produce discrete outcomes.

### Born Rule
Wavefunctions are probabilistic amplitude: at time $t$, the probability of finding the particle in the interval $(x, x +dx)$ is 
$$
dP(x,t) = |\Psi(x,t)^{2}|dx=\Psi^\star(x,t)\Psi(x,t)dx
$$
This is the Born Rule
Normalisation/Unitarity:
$$
1 = \int dP(x,t) = \int_{-\infty}^{\infty} |\Psi(x,t)^{2}| \, dx 
$$
Unitary implies particle number conservation
### Bra-ket Notation
Define ket states as column vectors:
$$
\ket{H} \equiv 
\begin{pmatrix}
1 \\
0
\end{pmatrix}
,
\ket{V} \equiv
\begin{pmatrix}
0 \\
1
\end{pmatrix}
$$
Then a $\theta$-direction ket state is
$$
\ket{\theta} = \cos \theta \ket{H} + \sin \theta \ket{V} =
\begin{pmatrix}
\cos \theta \\
\sin \theta
\end{pmatrix}
$$
A bra state is defined as the Hermitian (Dirac) conjugate of its corresponding ket state:
$$
\ket{\alpha} = 
\begin{pmatrix}
\alpha_{1} \\
\alpha_{2}
\end{pmatrix}
\Rightarrow
\bra{\alpha} \equiv (\ket{\alpha} )^{\dagger} \equiv 
\begin{pmatrix}
\alpha_{1}^\star \\
\alpha_{2}^\star
\end{pmatrix}
$$
Hermitian conjugate = Transpose + complex conjugate
### Polarisation States
#### Inner Product
The inner product between a pair of bra- and ket-states is calculated using matrix multiplication rules:
$$
\bra{\alpha}\ket{\beta} \equiv (\ket{\alpha} )^{\dagger}\ket{\beta} = \alpha_{1}^\star \beta_{1} + \alpha_{2}^\star \beta_{2}
$$
It is a complex number in general
Born rule: The above product of normalised states is a probability amplitude
Namely, its absolute square is the probability:
$$
P(\text{finding}\alpha \text{give} \beta) = |\bra{\alpha} \ket{\beta} |^{2}
$$
## Orthonormal Basis
Basis vectors are orthonormal (orthogonal and normalised):
$$
\bra{H} \ket{H} = 1= \bra{V} \ket{V} , \bra{H} \ket{V} = 0 = \bra{V} \ket{H}   \braket{V|H}  
$$
they form a complete basis set
That is, any state vector can be expressed as a linear combinatoin of the basis vectors:
$$
\ket{\alpha} = 
\begin{pmatrix}
\alpha_{1} \\
\alpha_{2}
\end{pmatrix}
= 
\alpha_{1}\ket{H} 
+ \alpha_{2}\ket{V}
$$
Polarised state $\ket{\theta}$ is normalised:
$$
\braket{\theta|\theta} \equiv (\ket{\theta} )^{\dagger}\ket{\theta} = \cos ^{2}\theta + \sin ^{2} \theta = 1  
$$
#### Classical vs. Quantum Description of Polarisation
Classical picture: When a light beam passes through a $\theta$-oriented polariser, it emerges as $\theta$-polarised light
Applying a subsequent horizontal polariser reduces the intensity by a factor of $\cos ^{2}\theta$
Quantum picture: For an initally $\theta$-polarised photon, the probability of detection after passing through a horizontal polariser is 
$$
P(\text{finding H given $\theta$}) = |\braket{H|\theta}|^{2} = \cos ^{2}\theta
$$
Same factor!
#### Change of Basis
Any linearly independent (and complete) set of vectors form a basis.
Among all possible basis choices, orthonormal sets prove most practical and mathematically convenient
For example, the $\theta$-direction polarisation and its perpendicular direction form an orthonormal basis:
$$
\ket{\theta} = \cos \theta \ket{H} +\sin \theta \ket{V}
$$
$$
\ket{\theta_{\perp}} \equiv \ket{\theta + \frac{\pi}{2}}  = -\sin \theta \ket{H} +\cos \theta \ket{V}
$$
They are orthonormal
$$
\braket{\theta|\theta} = 1 = \braket{\theta_{\perp}|\theta_{\perp}}, \braket{\theta|\theta_{\perp}}  =0
$$
#### Inverse Transformation
Conversely, each vector in the old basis can be written as a linear combination of the new basis vectors:
$$
\ket{\theta}  = \cos \theta \ket{H} +\sin \theta \ket{V}
$$
$$
\ket{\theta_{\perp}} = -\sin \theta \ket{H} + \cos \theta \ket{V}
$$
$$
\ket{H} = \cos \theta \ket{\theta} -\sin \theta \ket{\theta_{\perp}}
$$
$$
\ket{V} = \sin \theta \ket{\theta} +\cos \theta \ket{\theta_{\perp}}
$$
#### Completeness
For an arbitrary state $\ket{\alpha}=\cos \alpha \ket{H}+\sin \alpha \ket{V}$, we have
$$
\ket{\alpha}  = (\cos \alpha \cos \theta + \sin \alpha \sin \theta)\ket{\theta} + (-\cos \alpha \sin \theta+\sin \alpha \cos \theta)\ket{\theta_{\perp}}
$$
$$
= \cos(\alpha-\theta)\ket{\theta} + \sin(\alpha-\theta)\ket{\theta_{\perp}}
$$
#### Transformation of Quantum States
Wigner's Theorem: All transformations of quantum states must be linear and unitary
Linearity: The transformation preserves linear combinations
Unitarity: Inner products remain invariant uner transformation
Matrix Representation: Due to linearity, any transformation can be represented by a square matrix
Unitary condition: This matrix $U$ is unitary: $U^{\dagger}U = I$ where $I$ is the identity matrix
### Linear algebra in two dimension
## Puzzles of QM
### Schrodinger's cat
"Cat state"
$$
\Psi_{cat} = \frac{1}{\sqrt{ 2 }}(|alive\rangle + |dead \rangle)
$$
It's neither alive or dead
Recall polarisation of a photon:
$$
\Psi_{photon} = \frac{1}{\sqrt{ 2 }}(\ket{H} +\ket{V} )
$$
Can you say its $\ket{H}$ or $\ket{V}$ or both?

### Double-slit in QM
#### Waves vs Particles in Classical Physics
Waves -> interference
- Two coherent sources -> interference fringes
- Constructive interference: peaks align -> brighter
- Destructive interference: peaks in opposite phase -> cancels
Particles -> no interference
- Particles go through slit A or slit B
- Expected pattern on screen: two broad humps
- No alternating bright/dark fringes
#### Double-Slit with Single Quanta
Experiment setup 
- Source emits one electron/photon at a time
- Barrier with two narrow slits
- Distant screen detects impacts
Expectation from classical physics: Two humps
Observations
- Each detection is a single dot
- Dots accumulate into a pattern
- With both slits open: interference fringes
#### Classical particles
Probabilities add up in classical physics
With only one slit open, we observe a single peak
With both slits open, we observe a straightforward sum of two peaks
#### Quantum Particles
Each slit has a diffraction effect
Two slits have interference
$\text{Prob}_{A+B} \neq \text{Prob}_{A} + \text{Prob}_{A}$
Rather, $\Psi_{A+B} = \Psi_{A} + \Psi_{A}$
#### Path Detectors
Place detectors at slits to record "A" or "B"
Now each particle yields:
- a dot on screen
- plus a which-path record
Result:
- Interference fringes disappear
- Pattern becomes $\text{Prob}_{A}+\text{Prob}_{B}$
Explanation
- Interference needs coherence
- Observation destroy coherence
### Mach-Zehnder interferometer
#### Beam Splitter
A beam splitter is a semi-transparent mirror.
It reflects half of the incindent light and transmits the other half.
In bra-ket notation, a perfect beam splitter performs the transformation:
$$
\ket{1} \to \frac{1}{\sqrt{ 2 }}(\ket{3} +i\ket{4} ), \ket{2}  \to \frac{1}{\sqrt{ 2 }}(i\ket{3} +\ket{4} )
$$
The imaginary coefficients above are essential to ensure the transformation remains unitary, preserving probability conservation
#### Unitary Transformation
Re-labeling all horizontally propagating beams as $\ket{x}$ and vertically propagating beams as $\ket{y}$.
The previous transformation becomes
$$
\ket{x} \to \frac{1}{\sqrt{ 2 }}(\ket{x} +i\ket{y} ), \ket{y} \to \frac{1}{\sqrt{ 2 }}(i\ket{x} +\ket{y} )
$$
Matrix representation: 
$$
U = \frac{1}{\sqrt{ 2 }}
\begin{pmatrix}
1 & i \\
i & 1
\end{pmatrix}
$$
Clearly, it won't be unitary if all matrix elements are equal
#### Mach-Zehnder Interferometer
A Mach-Zehnder Interferometer consists of two beam splitters, two mirrors, and a transparent phase shifter placed in one arm
The first beam splitter splits the beam into two paths
The mirrors redirect the beams toward the second beam splitter, which recombines them
The phase shifter introduces an additional phase delay in one path
The second beam splitter can be removed to obtain which-path info
The outputs are measured by two detectors: $D_{1}$ for the $x$-port, and $D_{2}$ for the $y$-port
#### Math Modelling
Initial state: $\ket{x} = \begin{pmatrix}1 \\ 0 \end{pmatrix}$
Beam splitter:
$$
U = \frac{1}{\sqrt{ 2 }}\begin{pmatrix}
1 & i \\
i & 1
\end{pmatrix}
$$
Mirror: swaps the x and y modes
$$
M = \begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
$$
Phase shifter: adds phase only to x component:
$$
F = \begin{pmatrix}
e^{i\phi} & 0 \\
0 & 1
\end{pmatrix}
$$
#### A Photon Goes through MZI
After the 1st BS, the photon state becomes
$$
\frac{1}{\sqrt{ 2 }}
\begin{pmatrix}
1 \\
i
\end{pmatrix}
$$
Half in x path, half in y path (with a relative phase $\frac{\pi}{2}$)
Before the mirrors, the phase shifter acts as
$$
\frac{1}{\sqrt{ 2 }}\begin{pmatrix}
e^{i\phi} \\
i
\end{pmatrix}
$$
The mirrors then swap x and y components:
$$
\frac{1}{\sqrt{ 2 }}\begin{pmatrix}
i \\
e^{i\phi}
\end{pmatrix}
$$
#### Detecting Rates without the 2nd BS
Without the 2nd BS, $D_{1}$ detects the x-direction beam.
It will be triggered at the probability of
$$
|\frac{i}{\sqrt{ 2 }}|^{2} = \frac{1}{2} = 50\%
$$
Similarly, $D_{2}$ is triggered at the chance of 
$$
| \frac{e^{i\phi}}{\sqrt{ 2 }}|^{2} = \frac{1}{2} = 50\%
$$
#### Detecting Rates with the 2nd BS
If the 2nd BS is applied, the final state is
$$
\frac{1}{2}\begin{pmatrix}
i + ie^{i\phi} \\
-1 + e^{i\phi}
\end{pmatrix}
$$
$D_{1}$ detects at the rate of 
$$
\left| \frac{i}{2}(1 + e^{i\phi})\right|^{2} = \cos ^{2} \frac{\phi}{2}
$$
Similarly, $D_{2}$ detects at the rate of $\sin ^{2} \frac{\phi}{2}$
#### Delocalisation
Varying the extra phase $\phi$ changes the detecting outcomes
- If $\phi=0$, all photons exit in the x output
- If $\phi = \pi$, all photons exit in the y output
Changing $\phi$ in one arm changes the final state of every photon
The photon evolves as superposition of both paths
Delocalisation: The photon is delocalized across the interferometer
Delayed choice/quantum eraser: One may decide whether to insert the 2nd BS only after the photon has passed through the 1st BS - thereby choosing effectively, between observing interference (recombination) or retaining which-path information.
### Entanglement
Some two-photon states can be rewritten as products of two single-photon states.
For example,
$$
\ket{HV}  = \ket{H} \ket{V}
$$
$$
a\ket{HH} + b\ket{HV}  = \ket{H} (a\ket{H} +b\ket{V} )
$$
However, some two-photon states cannot be factorised.
For example,
$$
\frac{1}{\sqrt{ 2 }}(\ket{HH} + \ket{VV}  ) \neq (a_{1}\ket{H} +b_{1}\ket{V} )(a_{2}\ket{H} +b_{2}\ket{V} )
$$
A state that cannot be factorised in this way is called an entangled state.
### EPR paradox
Einstein, Podolsky, and Rosen proposed a thought experiment challenging QM in 1935.
Here is a modified version.
Two photons are prepared in the entangled state $\frac{1}{\sqrt{ 2 }}(\ket{HV}-\ket{VH})$, and they travel in opposite directions
If Alice measures the polarisation of Photon 1 and obtains $\ket{H}$, then she immediately knows that Bob must obtain $\ket{V}$ if he measures Photon 2, and vice versa.
Does this imply information propagates faster than the speed of light?
### No-cloning theorem
It is impossible to clone an unknown state without disturbing it
Suppose a physicist receives a photon in an unknown polarization state $\ket{\psi}$ and wants to prepare a second state with the same polarization.
To do so, he/she starts from a fixed "blank" state $\ket{R}$
One might hope to find a transformation such that
$$
\ket{R} \to T(\ket{R} ) = U\ket{R} = \ket{\psi}
$$
Equivalently, cloning would require a process of the form
$$
\ket{\psi} \ket{R}  \to \ket{\psi} \ket{\psi}
$$

#### Proof by Contradiction
Assume cloning is possible. Then for the basis states, we would have
$$
\ket{H} \ket{R}  \to \ket{H} \ket{H}
$$
$$
\ket{V} \ket{R} \to \ket{V} \ket{V}
$$
Now, lets try to clone the superposition state $\ket{+}= \frac{1}{\sqrt{ 2 }}(\ket{H}+\ket{V})$
We start with $\ket{+}\ket{R} = \frac{1}{\sqrt{ 2 }}(\ket{H}\ket{R}+\ket{V}\ket{R})$
By linearity, the cloning operation would give
$$
\ket{+} \ket{R}  \to \frac{1}{\sqrt{ 2 }}(\ket{H} \ket{H} + \ket{V} \ket{V} ) \neq \ket{+} \ket{+} 
$$
Hence, a universal cloning transformation cannot exist.
### Quantum teleportation
Although an unknown state cannot be cloned, it can be teleported
To do this, we use three photons
Photon A is prepared by Alice in an arbitrary polarization state:
$$
\ket{\theta} _{A} = \cos \theta \ket{H} _{A} + \sin \theta \ket{V} _{A}
$$
Photons B & C are prepared in an entangled state and sent to Alice and Bob, respectively:
$$
\ket{\Phi^{+}} _{BC} = \frac{1}{\sqrt{ 2 }}(\ket{H} _{B}\ket{H} _{C}+\ket{V} _{B}\ket{V} _{C})
$$
Alice performs a joint (Bell-state) measurement on Photons A & B.
This measurement projects A & B onto an entangled state and, in doing so, breaks the original entanglement between photons B & C.
#### Bell States
Bell States of two polarized photons:
$$
\ket{\Phi^+}  =  \frac{1}{\sqrt{ 2 }} (\ket{H} \ket{H} + \ket{V} \ket{V} )
$$
$$
\ket{\Phi^-}  =  \frac{1}{\sqrt{ 2 }} (\ket{H} \ket{H} - \ket{V} \ket{V} )
$$
$$
\ket{\Psi^+}  =  \frac{1}{\sqrt{ 2 }} (\ket{H} \ket{V} + \ket{V} \ket{H} )
$$
$$
\ket{\Psi^-}  =  \frac{1}{\sqrt{ 2 }} (\ket{H} \ket{V} - \ket{V} \ket{H} )
$$
They form an alternative (complete & orthonormal) basis for two photon states.
#### Bell-State Measurement
It can be shown that the three-photon state can be rewritten in the Bell basis states of A & B as
$$
\begin{align}
&\ket{\theta} _{A}\ket{\Phi^+} _{BC} \\
&= \frac{1}{2}\ket{\Phi^+} _{AB}(\cos \theta \ket{H} +\sin \theta \ket{V} )_{C} \\
&+ \frac{1}{2}\ket{\Phi^-} _{AB}(\cos \theta \ket{H} -\sin \theta \ket{V} )_{C} \\
&+ \frac{1}{2}\ket{\Psi^+} _{AB}(\sin \theta \ket{H} +\cos \theta \ket{V} )_{C} \\
&+ \frac{1}{2}\ket{\Psi^-} _{AB}(-\sin \theta \ket{H} +\cos \theta \ket{V} )_{C}
\end{align}
$$
Alice's Bell-state measurement on Photons A & B will collapse Photon C into the corresponding conditional state shown in (...)
#### Rearranging Photon States
$$
\begin{align}
\ket{\theta} _{A} \ket{\Phi^+} _{BC} &= (\cos \theta \ket{H} _{A}+\sin \theta \ket{V} _{A}) \frac{1}{\sqrt{ 2 }}(\ket{H} _{B}\ket{H} _{C}+\ket{V} _{B}\ket{V} _{C}) \\
&= \frac{1}{\sqrt{ 2 }}(\cos \theta \ket{HHH} + \cos \theta \ket{HVV} + \sin \theta \ket{VHH} + \sin \theta \ket{VVV}   ) \\
&= \frac{1}{\sqrt{ 2 }}\left[  \cos \theta  \frac{1}{\sqrt{ 2 }} \left(\ket{\Phi^+} _{AB}+ \ket{\Phi^-} _{AB})\right)\ket{H} _{C}+\cos \theta \frac{ 1}{\sqrt{ 2 }}  \right]
\end{align}
$$
#### Teleportation
Alice then sends Bob her Bell-state measurement results through a classical channel (only 2 bits info is needed).
Based on this result, Bob applies the corresponding unitary operation to Photon C.
After this correction, photon C is restored to exactly the same state that Photon A was in before the protocol.
Quantum teleportation does not violate special relativity, because completing the protocol requires classical communication, which cannot travel faster than light.
#### Unitary Transformation Needed by Bob
if Alice's result is Phi plus, yadda yadda yadda
#### A Brief History of Quantum Teleportation
Theoretical proposal: by Bennett, Brassard, Crepeau, Jozsa, Peres, & Wootters in 1993
First experimental demonstrations: independently by two groups, Popescu and Zeilinger in 1997
Platforms demonstrated: photons, atoms, electrons, superconducting circuits, etc
Record distance: Photon states have been teleported over 1,400 km using a satellite
Bennett & Brassard just won the Turing Award 2026 because of BB84 protocol for quantum key distribution
### Bell inequality
#### Bell Theorem (1964)
Consider a setup similar to the EPR scenario: Two photons are prepared in an entangled state and sent in opposite directions to Alice and Bob. 
Alice randomly chooses to measure Photon 1 is in either the $\ket{\alpha}$ basis or the $\ket{\alpha'}$ basis
She records the outcomes as $A_{0}=\pm 1$ for positive/negative $\ket{\alpha}$, and $A_{1}=\pm 1$ for positive/negative $\ket{\alpha'}$
Similarly, Bob randomly chooses to measure Photon 2 is in either $\ket{\beta}$ or $\ket{\beta'}$ polarisation. He records outcomes as $B_{0} =\pm 1$ or $B_{1} = \pm 1$
Bell theorem: if the photons carry fixed (predetermined) polarisations before measurements, then the correlations must satisfy the inequality:
$$
|\braket{A_{0}B_{0}} - \braket{A_{0}B_{1}} + \braket{A_{1}B_{0}} + \braket{A_{1}B_{1}}| \leq 2
$$
#### Proof of Bell Inequality
If the photons carry fixed (predetermined) polarizations, then Alice's outcomes are independent of Bob's measurement choice and outcome.
We can therefore analyse each run deterministically before taking ensemble average.
Regroup the expression:
$$
A_{0}B_{0} - A_{0}B_{1}+A_{1}B_{0}+A_{1}B_{1}=(A_{0}+A_{1})B_{0} - (A_{0}-A_{1})B_{1}
$$
Since both $A_{0}$ and $A_{1}$ can only take the values of $\pm 1$, we must have either $A_{0} = A_{1}$ or $A_{0} = -A_{1}$
Hence, one of the two parantheses, $(A_{0} + A_{1})$ or $(A_{0} + A_{1})$ must be zero
The remaining nonzero parantheses then equals + 2 or - 2
#### Proof of Bell Inequality
Multiplying the non-zero parentheses by $B_{0} = \pm 1$ or $B_{1} \pm 1$, the result is still $\pm 2$
Averaging over many trials may lead to partial cancellation between positive and negative contributions, but the magnitude of the averaged result cannot exceed 2
Therefore, if photons have predetermined polarisations before measurement, the Bell inequality must hold:
$$
| \langle A_{0}B_{0} - A_{0}B_{1} + A_{1}B_{0} + A_{1}B_{1} \rangle| = | \langle A_{0}B_{0} \rangle - \langle A_{0}B_{1} \rangle + \langle A_{1}B_{0} \rangle + \langle A_{1}B_{1} \rangle| \leq 2
$$
However, we will see that QM violates Bell inequality
#### Bell Inequality in QM
Consider two photons in the Bell state, $\ket{\Psi^-} = \frac{1}{\sqrt{ 2 }}(\ket{H}\ket{V}-\ket{V}\ket{H})$
Re-express the 1st photon state in the basis of $\ket{\alpha}$ & $\ket{\alpha^\perp}$, and the 2nd photon in $\ket{\beta}$ & $\ket{\beta^\perp}$, we get
$$
\ket{\Psi^-} = \frac{1}{\sqrt{ 2 }}[(\cos \alpha \ket{\alpha} -\sin \alpha \ket{\alpha_{\perp}} )(\sin \beta \ket{\beta} +\cos \beta \ket{\beta_{\perp}} ) - (\sin \alpha \ket{\alpha} +\cos \alpha \ket{\alpha_{\perp}} )(\cos \beta \ket{\beta} -\sin \beta \ket{\beta_{\perp}} )]
$$

$$
\ket{\Psi^-} = \frac{1}{\sqrt{ 2 }}(\sin \theta_{\alpha \beta} \ket{\alpha} \ket{\beta}  + \cos \theta_{\alpha \beta} \ket{ \alpha } \ket{\beta_{\perp}}  - \cos \theta_{\alpha \beta} \ket{ \alpha _{\perp}} \ket{ \beta_{\perp}}  + \sin \theta_{\alpha \beta} \ket{\alpha_{\perp}} \ket{\beta_{\perp}}  )
$$
where $\theta_{\alpha \beta} \equiv \beta-\alpha$
#### Probabilities
The probability amplitude of finding photon 1 in $\ket{\alpha}$ and photon 2 in $\ket{\beta}$ is
$$
\bra{\alpha} \bra{\beta} \Psi^- \rangle = \frac{\sin \theta_{\alpha \beta}}{\sqrt{ 2 }}
$$
By Born rule, the probability is 
$$
\text{Prob}_{\alpha \beta} = |\bra{\alpha} \bra{\beta} \Psi^- \rangle|^{2} = \frac{1}{2} \sin ^{2} \theta_{\alpha \beta}
$$
Similarly,
$$
\text{Prob}_{\alpha \beta_{\perp}} = |\bra{\alpha} \bra{\beta_{\perp}} \Psi^- \rangle|^{2} = \frac{1}{2} \cos ^{2} \theta_{\alpha \beta}
$$
$$
\text{Prob}_{\alpha_{\perp} \beta} = |\bra{\alpha_{\perp}} \bra{\beta} \Psi^- \rangle|^{2} = \frac{1}{2} \cos ^{2} \theta_{\alpha \beta}
$$
$$
\text{Prob}_{\alpha_{\perp} \beta_{\perp}} = |\bra{\alpha_{\perp}} \bra{\beta_{\perp}} \Psi^- \rangle|^{2} = \frac{1}{2} \sin ^{2} \theta_{\alpha \beta}
$$
#### Expectation Values
Therefore, the expectation value of $A_{0}B_{0}$ is
$$
\langle A_{0}B_{0} \rangle  = -\cos(2\theta_{\alpha \beta})
$$
#### Bell-CHSH Inequality
Similarly,
$$
\langle A_{0}B_{1} \rangle = -\cos(2\theta_{\alpha \beta}), \langle A_{1}B_{0} \rangle = -\cos(2\theta_{\alpha'\beta}), \langle A_{1}B_{1} \rangle = -\cos(2\theta_{\alpha'\beta'})
$$
Plugging in the LHS of Bell-CHSH inequality, we obtain,
$$
S \equiv \langle A_{0}B_{0} \rangle - \langle A_{0}B_{1} \rangle + \langle A_{1}B_{0} \rangle + \langle A_{1}B_{1} \rangle  = -\cos(2\theta_{\alpha \beta}) + \cos(2\theta_{\alpha \beta'} - \cos(2\theta_{\alpha'\beta}) - \cos(2 \theta_{\alpha'\beta'}))
$$
Note that not all $\theta$ are independent:
$$
\theta_{\alpha \beta'} = \beta' - \alpha = (\beta' - \alpha') + (\alpha' - \beta) + (\beta - \alpha) = \theta_{\alpha'\beta'} - \theta_{\alpha'\beta} + \theta_{\alpha \beta}
$$
Choose $\theta_{\alpha \beta} = - \theta_{\alpha'\beta}= \theta_{\alpha'\beta'} \equiv \theta$, we obtain $\theta_{\alpha\beta'} = 3\theta$ and a function
$$
S(\theta) = -3 \cos(2\theta) + \cos (6 \theta)
$$
#### QM Violates Bell Inequality
From the plot of $S(\theta)$, we can see there are regions that the Bell inequality is violated:
$$
|S| > 2
$$
The maximum violation occurs at $\theta = \frac{\pi}{8}, \dots$, giving
$$
|S|_{max} = |-3 \cos \frac{\pi}{4} + \cos \frac{3\pi}{4}| = 2\sqrt{ 2 } \approx 2.828
$$
