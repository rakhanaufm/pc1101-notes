# Complex Notation for Polarisation
An elegant mathematical treatment
Complex polarisation vector:
$$
\hat{\mathbf{e}}_{{\theta,\phi_{1},\phi_{2}}} \equiv \cos \theta e^{i\phi_{1}}\hat{\mathbf{e}}_{H} + \sin \theta e^{i\phi_{2}} \hat{\mathbf{e}}_{V}
$$
Any monochromatic wave becomes:
$$
\mathbf{E}(\mathbf{x},t) = E_{0} \mathrm{Re}\{e^{i(kz-\omega t) \hat{\mathbf{e}}_{\theta,\phi_{1}, \phi_{2}}}\}
$$
Advantage: separates amplitude, wave propagation, and polarisation

# Interference
Superposition of two light beams
## Constructive & Destructive Interference
$S_{1}$ and $S_2$ are two coherent wave sources
Consructive interference occurs when the path difference is an integral number of wavelengths
Destructive interference occurs when the path difference is a half-integral number of wavelengths

## Young's Double Slit
Milestone experiment by Thomas Young
Distance between aperture centers $d$
Observation distance is much larger than slit size $a$, separation, and wavelength
$$
R \gg a,d,\lambda
$$
Each aperture acts as a source of waves (Huygens' principle)
Waves interfere constructively or destructively depending on the path difference

## Narrow Apertures
Consider a very simple case with a narrow slit, separated by distance $d$, and the distance from the screen $R$
Fraunhofer approximation: if we take $R \to \infty$, we can treat the rays as parallel, in which case the path-length difference is simply $r_{2}-r_{1}=d\sin \theta$

Constructive interference:
$$
d\sin \theta=m\lambda
$$
Always occurs in forward direction 

Destructive interference:
$$
d\sin \theta=\left( m+ \frac{1}{2} \right) \lambda
$$
Complete cancellation of amplitude

## Amplitude of Interference
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

## Intensity
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

## Michelson Interferometer
Variable path: Moving mirror changes optical path
Path difference:
$$
\Delta l = 2(l_{1}-l_{2})
$$
(factor of 2 from reflection)
Historical applications:
	Michelson-Morley experiment
	LIGO gravitational wave detection: Nobel Prize 2017

## Coherence: Fundamental concept
Definition:
	Coherence: Stability in time of the relationship between two points in a wave
Two Main Types:
	Temporal (Longitudinal) Coherence: Relationship between $\psi(\textbf{x},t)$ and $\psi(\mathbf{x},t-\Delta t)$
	Spatial (Transverse) coherence: Relationship between $\psi(\mathbf{x}_{1},t)$ and $\psi(\mathbf{x}_{2},t)$
Measurement Method
	Use interferometry - unstable phase relationships wash out interference
## Longitudinal Coherence
Use wave packets as examples
Wave packet in interferometer:
	if delay $\Delta l >$ packet length, no interference
Coherence length $l_{c}$:
	Maximum delay for visible interference
coherence time:
$$
\tau_{c}= \frac{l_{c}}{c}
$$

## Transverse Coherence
Young's double slit with wavefront phase variations
Phase fluctuations across the wavefront: $\phi(\mathbf{x},t)$
Effect on Interference
	Stable wavefront: Clear interference fringes
	Fluctuating phases: Washed-out interference pattern
	Coherence length: Distance at which interference "disappears"
Measurement
	Vary slit separation $D$ to determine transverse coherence

## Diffraction
Finite apertures

## Huygens' Principle
Foundation for diffraction analysis
Key idea: Every point in space acts as virtual source of spherical wave
Applications:
	Build complex waves from spherical wave superposition
	Explain diffraction phenomena
	Predates Maxwell's equations but remains useful
Reality: Single emitters produce dipole waves (directional), but many emitters can approximate uniform spherical waves
Huygens' principle can be used to analyze diffraction
Fresnel diffraction: Source, screen, and obstacle are close together
Fraunhofer diffraction: Source, screen, and obstacle are far apart

## Single Slit

# Spherical Waves
Second common wave type
$$
\frac{A}{r(\mathbf{x})}\cos[kr(\mathbf{x})-\omega t+\phi]
$$
Where: $r(\textbf{x}) \equiv |\mathbf{x}-\mathbf{x}_{0}|= \sqrt{ (x-x_{0})^{2}+(y-y_{0})^{2}+(z-z_{0})^{2} }$
Wavefronts: Spheres centered at source $\textbf{x}_0$
Amplitude decay: $1/r$ from energy conservation
Energy conservation: Same energy spreads over larger sphere

## Optics
Light can be treated as rays: geometric optics
When wave effect is not negligible: physical optics
Problem: monochromatic plane wave hits slit of width $a$
Wave propagates in $\hat{x}$ direction
Slit width along $\hat{y}$ direction
Observe pattern at distance $R$ (far-field: $R \gg a$)

## Fraunhofer Diffraction
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

## Diffraction Result
Final result:
$$
E(\mathbf{x},t) = \frac{aA}{R} \cos(kR- \omega t) \text{sinc} \frac{ka\sin \theta}{2}
$$
Where: $\text{sinc}(\beta) \equiv \frac{\sin \beta}{\beta}$
Key feature: Amplitude depends on direction through $\text{sinc} \frac{ka\sin \theta}{2}$

$$
\Rightarrow I(\theta) \propto \text{sinc}^{2}\left( \frac{ka}{2}\sin \theta \right)
$$