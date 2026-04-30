# A Broken Reality
There exists an inequality, derived from very "reasonable" assumptions about how the world works, and that quantum mechanics violates. 

This is the CHSH inequality, and today we'll be forced to rethink what reality even means.
# Setup
Consider two particles prepared in an entangled state and sent far far apart.

Our two observers (Alice and Bob) each coose between two measurement settings:
- Alice: $a$ or $a'$
- Bob: $b$ or $b'$
Each measurement gives a binary outcome: $+1$ or $-1$.

Most importantly, their choices are independent, and no communication happens between the two.
# Assumptions
To describe this clasically, we assume:

Locality, that measurement outcomes here cannot be influenced instantly by distant choices.

Realism, that outcomes are predetermined by hidden variables $\lambda$, even before measurement.

Together this points to some sort of hidden variable, and these assumptions feel almost unavoidable in classical physics.

# Inequality
Define the correlation function:
$$
E(a,b) = \langle A(a)B(b) \rangle
$$
Now we can construct:
$$
S = E(a,b) + E(a,b') + E(a',b) - E(a',b')
$$
Under any local hidden variable model, one can prove:
$$
S \leq 2
$$
This here, is the CHSH inequality, which imposes a strict bound on classical correlations.
# Quantum Prediction
Take the entangled Bell state:
$$
\ket{\Phi^+}  = \frac{1}{\sqrt{ 2 }}(\ket{HH} + \ket{VV}  )
$$
Then choose measurement basis at specific relative angles. Quantum mechanics predicts that:
$$
S = 2\sqrt{ 2 }
$$
This, the Tsirelson bound, exceeds the classical limit. It's the maximum allowed by quantum theory.
# Experimental Results
This has been tested extensively using:
- Photons
- Ions
- Superconducting qubits
Modern Bell tests indeed confirm that:
$$
S > 2
$$
Nature consistently rejects local hidden variable theories (and papers).
