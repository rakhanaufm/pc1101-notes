# Physical Interpretation
When do we see rays vs diffraction?
Small aperture $(a \ll \lambda)$:
	$\text{sinc}\left( \frac{ka}{2}\sin \theta \right) \approx 1, \forall \theta$
	Uniform spherical wave (point source behavior)
Large aperture $(a \gg \lambda)$
	$\text{sinc}\left( \frac{ka}{2}\sin \theta \right) \approx 0$ unless $0 \ll \frac{\lambda}{a}$
	Light concentrated in forward direction -> ray behavior
conclusion: geometric optics emerges when aperture >> wavelength

# Rayleigh Diffraction Limit
## Resolution of Optical Systems
Question: Can we distinguish two sources separated by distance $q$?
Rayleigh criterion: Sources just resolved when peak of one conicides with first zero of the other's diffraction pattern
For circular aperture: $q \approx 1.22 \frac{R \lambda}{a}$
	$R$: distance to sources
	$a$: aperture diameter
	$\lambda$: wavelength

## Applications and Implications
Telescope resolution:
	Larger aperture -> better resolution
	Hubble Space Telescope: 2.4 m aperture
Camera phones:
	Small aperture limits resolution
	Computational photography compensates
Microscopy:
	Shorter wavelength -> better resolution
	Electron microscopes use $\lambda \ll$ visible light
Diffraction-limited: System limited by physics, not imperfections

# Propagation of Light in Media
Understanding how light behaves when it enters different materials
## Light slows down in dense media
In a homogeneous isotropic medium,
$c \to v = \frac{c}{n}$
where:
	$c$ = speed of light in vacuum
	$n$ = refractive index
For slowing down: $n > 1$
Key insight: the frequency remains unchanged, but wavelength becomes shorter

## Dispersion Relation
Refractive index depends on frequency: $n= n(\omega)$
In vacuum: $\omega = ck_{0}$
In a medium, the frequency is unchanged: $\omega = v(\omega)k_{n}(\omega)$
Where the speed in the medium: $v(\omega) = \frac{c}{n(\omega)}$
Wave number: $k_{n}(\omega) = n(\omega)k_{0} = n(\omega) \frac{\omega}{c}$

## Microscopic Origin of Refractive Index
Light incidents on atoms
Make electrons vibrate
Vibrating charges emit light
Electrons oscillate at driving frequency
Accumulated delays -> slowing down
Model: Driven damped oscillator

### Recall: Driven Damped Oscillator Model
Newton's equation:
$$
m \frac{d^{2}x}{dt^{2}} = -kx - m \gamma\frac{ dx}{dt} + F_{0} \cos(\omega t)
$$
Three forces:
	spring force: $F_{osc} = -kx = -m\omega_{0}^{2}x$
	Damping force: $F_{damp} = -m \gamma v = -m \gamma  \frac{dx}{dt}$

Solution of Oscillator
Complex form:
$$
\frac{d^{2}z}{dt^{2}} + \gamma  \frac{dz}{dt} + \omega_{0}^{2}z = \frac{F_{0}}{m}e^{-i\omega t}
$$
Ansatz:
$$
z(t) = A(\omega)e^{i[-\omega t + \phi(\omega)]}
$$
Quiz07: solve the equation using the ansatz and verify the results:

## From Atoms to Medium
Key insight: Phase accumulates atom by atom
Total phase over distance $x$: $\phi(\omega,x)= \frac{x}{a} \phi(\omega)$
Where $a$ is the typical distance between atoms
Recall the phase factor of a planewave
$$
e^{i(k_{0}x-\omega t+\phi(\omega ,x))} \equiv e^{i[n(\omega)k_{0}x-\omega t]}
$$
Refractive index formula:
$$
n(\omega) - 1 = \frac{c}{a} \frac{\phi(\omega)}{\omega}
$$
### Back of Envelope Calculation
Estimation of parameters:
	$c \approx 3 \times 10^8$ m/s
	$a \approx 10^{-10}$ m
	for visible light: $\omega \approx 2\pi \times 500 \text{THz} \approx 3 \times_{1}0^15$ 1/s
the coefficient in front of $\phi(\omega) = \frac{c}{a\omega} \approx 10^{3}$
Far away from resonance, $n(\omega)$ is of order 1, this means that
$$
\phi(\omega) \ll 1
$$
$$
\Rightarrow \phi(\omega) \approx \tan \phi(\omega) = \frac{\gamma\omega}{\omega^{2}-\omega_{0}^{2}}
$$
### Far away from resonance
Far below resonance: $\omega \ll \omega_{0}$
$$
\Rightarrow n(\omega)\approx 1 + \frac{c\gamma}{a\omega_{0}^{2}} \frac{1}{1- \frac{\omega^{2}}{\omega_{0}^{2}}} \approx 1 + \frac{c\gamma}{a\omega_{0}^{2}} \left( 1 + \frac{\omega^{2}}{\omega_{0}^{2}} \right)
$$
Far above resonance: $\omega \gg \omega_{0}$
$$
\Rightarrow n(\omega) \approx 1 + \frac{c\gamma}{a\omega_{0}^{2}} \frac{1}{1 - \frac{\omega^{2}}{\omega_{0}^{2}}} \approx 1
$$
## Sellmeier's Equation
More complete model with multiple resonances:
$$
n^{2}(\omega) = 1 + \sum_{i} \frac{B_{i}}{1-\left( \frac{\omega}{\omega_{i}} \right)^{2}}
$$
Below all resonances $(\omega \ll \omega_{i} \forall i)$:
$$
n^{2}(\omega) \approx 1 + B_{1} + B_{2} + \cdot \cdot \cdot
$$
Between resonances: Terms drop out progressively
For example if $\omega_{1} \ll \omega\ll \omega_{2}$, then
$$
\frac{1}{1-\left( \frac{\omega}{\omega}1 \right)^{2}} \to 0 \Rightarrow n^{2}(\omega) \approx  1 + B_{2} + \cdot \cdot \cdot
$$
High frequency limit: $\omega \gg \omega_{i} \forall i$

## Extensions and Advanced Topics
Complex refractive index:
$$
n(\omega) = n_{r}(\omega) + in_{i}(\omega)
$$
	Real part: phase velocity
	Imaginary part: attenuation
Other phenomena:
	Birefringence: $n$ depends on polarization
	Nonlinear optics: Response at different frequencies
	Negative index: $n<0$ in metamaterials
	Sub-unity index: $n<1$ for x-rays, some metals

# Wave Packets in Media
Each frequency component evolves independently:
$$
\psi(x,t) = \frac{1}{\sqrt{ 2\pi }} \int_{-\infty}^{\infty} \tilde{\psi} (k) e^{i[n(\omega)k_{0}x-\omega t]} \, dt, \omega = ck_{0}
$$

## Different Velocities
Recall the dispersion relation:
$$
|\mathbf{k}(\omega)| \equiv n(\omega)k_{0} = \frac{n(\omega)\omega}{c}
$$
Three important velocity concepts:
	1. Phase velocity: Speed of wave crests
$$
v_{\phi}(k) = \frac{\omega}{k}
$$
	2. Group velocity: Speed of wave packet envelope
$$
v_{g}(k) = \frac{d\omega(k)}{dk}
$$
	3. Front velocity: Speed of information transfer
$$
v_{f} \leq c
$$
## Interface Phenomena
At the boundary between two media, two laws govern behaviour
**Reflection**: 
$$
\theta_{r}=\theta_{i}
$$
**Refraction (Snell's Law)**:
$$
n_{t}\sin \theta_{t} = n_{i} \sin \theta_{i}
$$
## Snell's Law Details
Key observations:
	If $n_{t} >n_{i}$: beam bends towards normal
	If $n_{t}<n_{i}$: beam bends away from normal
Special case - Total Internal Reflection (TIR):
	When $n_{t}<n_{i}$, for large enough incidence angle $\theta_{i} \in [\theta_{i}^{TIR}, \frac{\pi}{2})$ with $\sin \theta_{i}^{TIR} \equiv \frac{n_{t}}{n_{1}}$ there is no transmission.
Application: Optical fibres!

## Fermat's Principle
One classical way to derive Snell's law
**Fermat's Principle**: Light takes the path of shortest time (or shortest optical path)
**Math:** to minimize
$$
T = \frac{n_{1}}{c} \sqrt{ a^{2} +l_{1}^{2} } + \frac{n_{2}}{c} \sqrt{ b^{2} + (l-l_{1})^{2} }
$$
