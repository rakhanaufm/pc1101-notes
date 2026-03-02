# Continuum Theory
The Klein-Gordon Lagrangian in 2+1D:
$$
\mathcal{L} = \frac{1}{2}(\partial_{t}\phi)^{2} - \frac{1}{2} (\nabla \phi)^{2} - \frac{1}{2} m^{2} \phi^{2}
$$
Euler-Lagrange then gives:
$$
\partial_{t}^{2}\phi - \nabla^{2}\phi + m^{2}\phi = 0
$$
This is the relativistic massive wave equation, which yields plane wave solutions:
$$
\phi \sim e^{-i\omega t + i \mathbf{k}\cdot \mathbf{x}}
$$
Plugging this into the previous equation yields,
$$
\omega^{2} = \mathbf{k}^{2} + m^{2}
$$
This is the continuum dispersion relation. This shows that having mass gives an energy gap at $k=0$.
# Canonical Hamiltonian
Now let's define the conjugate momentum:
$$
\pi = \frac{\partial\mathcal{L}}{\partial(\partial_{t}\phi)} = \partial_{t}\phi
$$
The Hamiltonian density is thus,
$$
\mathcal{H} = \frac{1}{2}\pi^{2} + \frac{1}{2}(\nabla \phi)^{2} + \frac{1}{2}m^{2}\phi^{2}
$$
So then the energy is:
$$
H = \int d^{2}x\left[\frac{1}{2}\pi^{2} + \frac{1}{2} (\nabla \phi)^{2} + \frac{1}{2}m^{2}\phi^{2}\right]
$$
The interpretation of this is
	$\pi^{2}$ -> kinetic energy
	$(\nabla \phi)^{2}$ -> spatial coupling
	$m^{2}\phi^{2}$ -> local restoring force
# Lattice Discretization
Now let's discretize space, such that
$$
x = ia, \space \space \space y=ja
$$
We can now replace the gradients with finite differences:
$$
\nabla^{2}\phi \to \frac{1}{a^{2}} (\phi_{i+1,j} + \phi_{i-1,j} + \phi_{i,j+1} + \phi_{i,j-1} - 4\phi_{i,j})
$$
The lattice Hamiltonian then becomes,
$$
H = \sum_{i,j} \left[\frac{1}{2}\pi^{2}_{i,j} + \frac{1}{2}m^{2}\phi^{2}_{i,j} + \frac{1}{2a^{2}}\left((\phi_{i+1,j} - \phi_{i,j})^{2} + (\phi_{i,j+1}-\phi_{i,j})^{2}\right)\right]
$$
This is a 2D array of coupled harmonic oscillators.
# Fourier Diagonalization
We first define the discrete Fourier transform,
$$
\phi_{i,j} = \frac{1}{N}\sum_{k_{x},k_{y}} \tilde{\phi}_{k_{x},k_{y}} e^{i(k_{x}ia+k_{y}ja)}
$$
Plug this into the Hamiltonian, then we get that the cross terms cancel, each mode decouples, giving us the result:
$$
H = \sum_{k_{x},k_{y}}\left[\frac{1}{2}|\tilde{\pi}|^{2} + \frac{1}{2} \omega^{2}_{k} |\tilde{\phi}_{k}|^{2}\right]
$$
where
$$
\omega_{k}^{2} = m^{2} + \frac{4}{a^{2}}\left[\sin ^{2}\left(\frac{k_{x}a}{2}\right) + \sin ^{2} \left(\frac{k_{y}a}{2}\right)\right]
$$
Each momentum mode is an independent harmonic oscillator.

# Continuum Limit
For small $k$:
$$
\sin\left( \frac{ka}{2} \right) \approx \frac{ka}{2}
$$
So:
$$
\omega^{2} \approx m^{2} + k^{2}_{x} + k^{2}_{y}
$$
We thus recover the relativistic dispersion relation. The lattice is a UV regulator which ensure UV completeness.
# Vacuum Correlation Function
The ground-state 2-point function is:
$$
\langle \phi_{0,0}\phi_{i,j} \rangle  = \frac{1}{N^{2}}\sum_{k_{x},k_{y}} \frac{1}{2\omega_{k}} e^{i(k_{x}ia + k_{y}ja)}
$$
For large distance:
	$m=0$ -> algebraic decay
	$m>0$ -> exponential decay
Correlation length:
$$
\zeta \sim \frac{1}{m}
$$
Mass gap = finite correlation length.
# Quantization
Let's promote modes to become operators:
$$
[\tilde{\phi}_{k}, \tilde{\pi}_{k}] = i\delta_{k,k'}
$$
We will also define creation operators:
$$
a_{k} = \sqrt{ \frac{\omega_{k}}{2} }\tilde{\phi}_{k} + \frac{1}{\sqrt{ 2\omega_{k} }}\tilde{\pi}_{k}
$$
The Hamiltonian then becomes:
$$
H = \sum_{k}\omega_{k}\left( a^{\dagger}_{k}a_{k} + \frac{1}{2} \right)
$$
We can thus conclude that particles are quanta of these normal modes.
