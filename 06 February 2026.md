# Scattering Overview
Three regimes based on scatterer size $a$ vs. wavelength $\lambda$
**Rayleigh Scattering** $(a \ll \lambda)$
	Example: blue sky
	Cross-section $\propto \frac{1}{\lambda^4}$
**Mie Scattering** $(a \approx \lambda)$
	Example: Fog, haze
	Complex, depends on details
**Geometric Scattering** $(a\gg \lambda)$
	Example: shadows
	Ray optics applies

## Simple Model for Rayleigh Scattering
Driven oscillator again:
$$
m_{e} \frac{d^{2}x}{dt^{2}} + m_{e} \gamma \frac{ dx}{dt} + m_{e} \omega_{0}^{2}x = -eE_{0}e^{-i\omega t}
$$
Results amplitude:
$$
A(\omega) = \frac{\left( -\frac{eE_{0}}{m_{e}} \right)}{\sqrt{ (\omega^{2}-\omega_{0}^{2})^{2} + \gamma^{2}\omega^{2} }}
$$
Radiation intensity $\propto$ acceleration^2 $\propto$ $|-\omega^{2}A(\omega)|^{2} \propto \frac{\omega^4}{(\omega^{2}-\omega_{0}^{2})^{2} + \gamma^{2}\omega^{2}}$

### Limiting Cases
Free charges $\Rightarrow$ Thomson scattering: $\omega \gg \omega_{0}, \gamma$
$$
\text{Denominator} \approx (\omega^{2})^{2} + \gamma^{2}\omega^{2} = \omega^{2}(\omega^{2}+\gamma^{2}) \approx \omega^{2}\omega^{2} = \omega^4
$$
$$
\text{Radiation} \propto \frac{\omega^4}{\omega^4} \approx 1
$$
$\Rightarrow$ scattering is independent of $\omega$
Bounded charges $\Rightarrow$ Rayleigh scattering: $\omega_{0} \gg \omega, \gamma$
$$
\text{Denominator} \approx \omega_{0} + \gamma^{2}\omega^{2} \approx \omega_{0}^4
$$
$$
\text{Radiation} \propto \frac{\omega^4}{\omega_{0}^4} \propto \frac{c^4}{\omega_{0}^4 \lambda^4} \propto \frac{1}{\lambda^4}
$$
$\Rightarrow$ scattering $\propto \omega^4 \frac{\propto_{1}}{\lambda^4}$

# Measuring the Speed of Light
Romer's measurement (1676)
	Observing the eclipses of Io
	His result is about 3/4 of true value.
Fizeau's experiments (1849)

## If Light is a Wave...
Then what is oscillating?
Sound waves: disturbance or vibration in a medium of solid, liquid, or gas (elastic media) and it follows that wehere there is no medium ther is no douns
Water waves: water molecules move up and down
Light waves: ???
	Answer in the 19th century: Aether
## The Aether
Aether, or sometimes spelled "ether", was the hypothetical substance through which electromagnetic waves travel. It was used by several optical theories as a way to allow propagation of light, which was believed to be impossible in "empty" space.

It was supposed that the ether filled the whole Universe and was a stationary frame of reference, which was rigid to electromagnetic waves but completely permeable to matter.

### Suppose Aether Exists...
The earth is moving relative to the aether
$v$ of light measured on Earth = $v$ of light + $v$ of Earth relative to aether

### Michelson-Morley Experiment (1887)
If there is motion of Earth relative to the aether, then the observed speed of light should be different for light in different directions
Michelson & Morley used their interferometer and found ..
$$
\text{NOTHING}
$$
Speed of light is the same in any direction $\approx$ 300,000 km/s
Either Newtonian Mechanics or Maxwell's Equations had to be modified

# Einstein's Resolution
The principle of relativity holds for E&M: Maxwell's Equations are right
The speed of light has the same value $c$ in all inertial frames
![[Pasted image 20260206111124.png]]
Changing Newtonian Mechanics
Changing the concepts of space and time

## The Ultimate Speed - Experiment
1964 at CERN in Geneva, Switzerland
W. Bertozzi and coworkers accelerated electrons to various measured velocities and with independent methods measured their kinetic energies
Result: The kinetic energy increases toward very high values but doesnt surpass the speed of light

## Testing the Speed of Light Postulate
Also 1964 at CERN in Geneva, Switzerland
T. Alvaeger and co-workers measure the decay of the neutral pion $\pi^0$ moving at a high velocity
$$
\pi^0 \to \gamma + \gamma
$$
$\gamma$ rays are electromagnetic waves with very high frequency (and of course velocity $c$)
Result: the rays are 

# SR vs. GR: Similarities

| Special Relativity                                                                                       | General Relativity                                                           |
| -------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| Einstein (1905)                                                                                          | Einstein (1916)                                                              |
| Physical laws are the same in all inertial reference frames, but they may vary across non-inertial ones. | Physical laws are the same in all reference frames, inertial or non-inertial |
| What happens when we move fast                                                                           | What happens when we are close to a big mass                                 |

# SR vs. GR: Differences

| Special Relativity                                          | General Relativity                                      |
| ----------------------------------------------------------- | ------------------------------------------------------- |
| Einstein + Lorentz + Poincare                               | Einstein alone, a state-of-art work                     |
| Principles which all physical theories should obey, like QM | The theory about a fundamental force of nature: gravity |
| More or less completed: compatible with QM -> QFT           | Obviously incomplete: no quantum gravity, yet           |

# Space & Time in Newtonian Mechanics
## Measuring an Event
An event is something that happens, and every event can be assigned three space coordinates and one time coordinate
Among possible events are the collision of two particles, a flash of light, the passage of a laser beam through a specific point, an explosion, ...
The coordinates characterizing an event are called spacetime coordinates
Different observers in different reference frames will assign different spacetime coordinates

## Reference Frame
What is a reference frame?
A particular perspective from which the universe is observed. Imagine a set of axes from which an observer can measure the position and motion of all points in the system. and a clock

## Moving Reference Frame
Person walking with a velocity $v_{w}$, as measured by an observer moving along with him on the walkway
Walkway surface moves with $v_{wt}$ relative to terminal
Two velocities add as vectors
Velocity of person as measured by someone standing in the terminal:
$$
v_{t} = v_{w} + v_{wt}
$$
## Lab Frame
Consider a world containing free particles, moving this way and that
To describe and understand the motions of the particles:
The laboratory defines a reference frame (coordinate system).

## Inertial Frame
There are many possible laboratories, which can be
	moving uniformly wrt each other
	accelerating wrt each other
	rotating wrt each other
	or some combination
Not all these ref frames are equally useful for expressing the laws of mechanics

## Construction of Inertial Frames
Pick a free particle to serve as the origin of a Cartesian coordinate system at all times.
propagate the initial axes parallel to themselves

## Time
An observer in an inertial frame can discover a parameter $t$ with respect to which the positions of all free particles are changing at constant rates:
$$
x(t) = x_{0} + v_{x}t, \space y(t) = y_{0} + v_{y}t, \space z(t) = z_{0} + v_{z}t
$$
$t$ is time.
An inertial observer can construct a clock that measures $t$: the position of one free particle could be used to measure $t$, since its position changes at a constant rate in $t$.

