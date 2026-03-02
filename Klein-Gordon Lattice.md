# 2D Klein-Gordon Field
At its core, the Klein-Gordon field is just a massive wave equation. Which in continuous space, looks like:
$$
\partial_{t}^{2}\phi = \nabla^{2} \phi - m^{2}\phi
$$
That's it. With conditions,
	If $m=0$ -> pure wave equation
	If $m>0$ -> waves that resist oscillation (mass gap)

# Let's Make This Discrete
Instead of a continous space, now imagine a two dimensional grid.
Each grid point has a number:
$$
\phi _{i,j}
$$
Each point has the following properties,
	It oscillates like a harmonic oscillator
	It is coupled to its neighbors
	And it feels a restoring force from its mass
Thus, the Hamiltonian becomes,
$$
H = \sum_{i,j} \left[\frac{1}{2}\pi^{2}_{i,j} + \frac{1}{2} m^{2} \phi^{2}_{i,j} + \frac{1}{2a^{2}}(\nabla_{lattice}\phi)^{2}\right]
$$
Which we can interpret as a 2D sheet of coupled springs. Now, that's a quantum field.

# Normal Modes
If we then Fourier transform the grid, everything diagonalizes.
The frequencies are:
$$
\omega^{2}(k_{x},k_{y}) = m^{2} + \frac{4}{a^{2}}\left[\sin ^{2}\left( \frac{k_{x}a}{2} \right) + \sin ^{2}\left(\frac{k_{y}a}{2}\right)\right]
$$
This tells us the dispersion relation.
We can interpret this as,
	Long wavelengths -> low frequency
	Short wavelengths -> high frequency
	Mass shifts everything upward
When $m>0$, the system has a mass gap.
No zero-frequency mode, and the gap is the correlation length.

# The Significance
This simple model connects quantum fields, phonons in solids, correlation functions, phase transitions, and lattice QFT. 
This shows that a "particle" in quantum field theory is just a quantized normal mode of this field. 
I think this is incredibly beautiful, it gives a very strong intuition into the wave-particle duality in quantum mechanics. 
Therefore, I have thus made a small project plotting the different behaviors represent by the Klein-Gordon field.