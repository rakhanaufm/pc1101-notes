# How Atoms/Molecules Interact with Light?
## Structure of atoms:
- Neutral overall but contains charged components
- Nuclei(positive) + Electrons(negative)
## Electric Dipole Formation:
- Electric field separates charge centers
- Creates oscillating dipole when field varies
- Dipole oscillation frequency = field frequency

# Dielectrics vs Metals
## Dielectric Materials
- Bound electrons form dipoles
- Transparent to light
- Light propagates through material
## Metals
- Free electrons shared among atoms
- Absorb light -> electronic motion -> heat
- Not transparent

Course focus: Dielectric materials only

# Light-Matter Interaction Mechanism
## The Basic Process:
Light -> Oscillating Dipole -> Scattered Light

## Key Features:
- Light makes dipole oscillate
- Oscillating dipoles emit light (act as antennas)
- Spherical wave emission (all directions)
- Same frequency as incident light

This is the fundamental mechanism of light-matter interaction

# Oscillations
## Simple Harmonic Motion (SHM)
### Simple Harmonic Motion:
$$
\ddot{f}(t) = -\omega^2f(t)
$$
It is a constant coefficient 2nd-order ordinary differential equation
- It can be solved by an exponential function
Where $\omega$ is called angular frequency, $rad/s$

### Solving $\ddot{f}(t) = -\omega^2f(t)$ 
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

### Alternative solutions
$$
f_{2}(t) = D_{1}\cos(\omega t) + D_{2}\sin(\omega t)
$$
$$
\dot{f_{2}} = -D_{1}\omega \sin(\omega t) + D_{2}\omega \cos(\omega t) \Rightarrow \ddot{f_{2}} = -D_{1}\omega^2\cos(\omega t) - D_{2}\omega^2\sin(\omega t) = -\omega^2 f_{2}
$$
$$
f_{3}(t)=A\cos(\omega t + \phi)
$$
$$
\dot{f_{3}}=-A\sin(\omega t + \phi)\frac{d}{dt}(\omega t + \phi) = -A \omega \sin(\omega t + \phi)
$$
$$
\ddot{f_{3}} = -A \omega^2 \cos(\omega t+\phi) = -\omega^2f_{3}
$$
$A$ is called the amplitude, and $\phi$ is a phase
### Remarks on Phases
For a single SHM,
$$
f(t) = A\cos(\omega t + \phi)
$$
Any phase $\phi$ can be absorbed by shifting $t \rightarrow t - \frac{\phi}{\omega}$
- There is no physical meaning to the global phase of a wave
- The relative phases matter for two or more such waves
We can also use the sine function by shifting the phase by 90 deg.

## Complex Notation Advantages
Using Euler's formula:
$$
e^{i \theta} = \cos(\theta) + i\sin(\theta)
$$
SHM in complex form:
$$
\cos(\omega t+\phi) = \mathrm{Re}\left(e^{i \omega t}e^{i\phi}\right)
$$
Advantages:
- Adding phase becomes simple multiplication
- Superposition preserved
- Calculations much simpler

Caution: For intensity, use real parts first!

### Trigonometric Formulas Are Easy
Open up $e^{i(\alpha + \beta)} = e^{i\alpha}e^{i\beta}$ to obtain immediately the formulas for $\cos(\alpha + \beta)$ and $\sin(\alpha + \beta)$ without the need to memorize them.
$$
\begin{align} 
\text{Euler's Formula}& \Rightarrow \cos_(\alpha + \beta) + i\sin(\alpha + \beta) \\
& = [\cos(\alpha) + i\sin(\alpha)][\cos(\beta)+i\sin(\beta)] \\
& = \cos(\alpha)\cos(\beta) + i\sin (\alpha)\cos(\beta) + i\cos(\alpha)\sin(\beta) - \sin(\alpha)\sin(\beta) \\
& = [\cos (\alpha)\cos(\beta)-\sin(\alpha)\sin(\beta)] + i[\sin(\alpha)\cos(\beta)+\cos(\alpha)\sin(\beta)] \\
\mathrm{Re\{Equation\}} & \Rightarrow \cos(\alpha + \beta) = \cos(\alpha)\cos(\beta) -\sin(\alpha)\sin(\beta) \\
\mathrm{Im\{Equation\}} & \Rightarrow \sin(\alpha + \beta) = \sin(\alpha)\cos(\beta) + \cos(\alpha)\sin(\beta)
\end{align} 
$$

## Beat Phenomena
Two oscillations with same amplitude, different frequencies:
$$
\psi(t) = A\cos(\omega_{1}t)+A\cos(\omega_{2}t)
$$
Remember that,
$$
\cos(\alpha+\beta) = \cos(\alpha)\cos(\beta)-\sin(\alpha)\sin(\beta)
$$
$$
\cos(\alpha-\beta)=\cos(\alpha)\cos(-\beta)-\sin(\alpha)\sin(-\beta) = \cos(\alpha)\cos(\beta)+\sin(\alpha)\sin(\beta)
$$
If we add the two equations together,
$$
\Rightarrow \cos(\alpha+\beta)+\cos(\alpha-\beta)=2\cos(\alpha)\cos(\beta)
$$
$$
\alpha + \beta = \omega_{1}t, \alpha-\beta=\omega_{2}t
$$
This can be solved for $\alpha$ and $\beta$
$$
\alpha=\frac{\omega_{1}+\omega_{2}}{2}t,\beta=\frac{\omega_{1}-\omega_{2}}{2}t
$$
Hence,
$$
\psi(t)=2\cos(\frac{\omega_{1}+\omega_{2}}{2}t)\cos(\frac{\omega_{1}-\omega_{2}}{t})
$$
If $\omega_1 \approx \omega_2$ , we can write them as $\omega_1=\Omega + \delta$ and $\omega_2 = \Omega - \delta$ with $\delta << \Omega$
$$
\Rightarrow \psi(t) = 2\cos(\Omega t)\cos(\delta t)
$$
Becomes an enveloped equation
![[Pasted image 20260120110544.png]]
## Damped Oscillation
Oscillation with damping:
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
### Verification of Solutions
$$
f(t)=C_{1}e^{-\beta t}e^{i\omega t}+C_{2}e^{-\beta t}e^{-i\omega t}
$$
$$

\begin{align}
\dot{f}& =C_{1}(-\beta+i\omega)e^{(-\beta+i\omega)t} + C_{2}(-\beta - i\omega)e^{(-\beta - i \omega)t} \\
\ddot{f} &= C_{1}(-\beta+i\omega)^2e^{(-\beta+i\omega)t}+C_{2}(-\beta-i\omega)^2e^{(-\beta-i\omega)t} \\
\text{LHS} & = C_{1}(-\beta+i\omega)^2e^{(-\beta+i\omega)t}+C_{2}(-\beta-i\omega)^2e^{(-\beta-i\omega )t}+2\beta[C_{1}(-\beta+i\omega)e^{(-\beta+i\omega)t}+C_{2}(-\beta-i\omega)e^{(-\beta-i\omega)t}] \\ \\
& = C_{1}[(-\beta+i\omega)^2+2\beta(-\beta+i\omega)+\omega_{0}^2]e^{(-\beta+i\omega)t}+C_{2}[(-\beta-i\omega)^2 + 2\beta(-\beta-i\omega)+\omega_{0}^2]e^{(-\beta-i\omega)t} \\
[\space \space \space \space \space] & = (-\beta+i\omega)^2+2\beta(-\beta+i\omega)+\omega_{0}^2 \\
& = \beta^2-2i\beta \omega-\omega^2 -2\beta^2 +2i\beta \omega +\omega_{0}^2 \\
& = -\omega^2 -\beta^2 +\omega_{0}^2 \space \space \text{with} \space \space \omega^2 = \omega_{0}^2-\beta^2\\
& = -\omega_{0}^2 +\beta^2 -\beta^2 +\omega_{0}^2 \\
& = 0
\end{align}
$$

### Classification of Damping
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
