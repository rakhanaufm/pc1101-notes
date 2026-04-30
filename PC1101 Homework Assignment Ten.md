# 1. Entanglement Swapping
$$
\ket{\Psi^{+}}_{DA} = \frac{1}{\sqrt{ 2 }}(\ket{H} _{D}\ket{V} _{A}+\ket{V} _{D}\ket{H} _{A})
$$
$$
\ket{\Psi^{+}} _{BC} = \frac{1}{\sqrt{ 2 }}(\ket{H} _{B}\ket{H} _{C}+\ket{V} _{B}\ket{V} _{C})
$$
a)
Then the full 4-photon state is 
$$
\ket{\Psi} _{DABC} = \frac{1}{2}\left(\ket{H} _{D}\ket{V} _{A}\ket{H} _{B}\ket{H} _{C} + \ket{H} _{D}\ket{V} _{A}\ket{V} _{B}\ket{V} _{C} + \ket{V} _{D}\ket{H} _{A}\ket{H} _{B}\ket{H} _{C} + \ket{V} _{D}\ket{H} _{A}\ket{V} _{B}\ket{V} _{C}\right)
$$
Using these, which we derived in 10th of April lecture quiz,
$$
\ket{HH}  =  \frac{1}{\sqrt{ 2 }} (\ket{\Phi^+}  + \ket{\Phi^-} )
$$
$$
\ket{HV}  =  \frac{1}{\sqrt{ 2 }} (\ket{\Psi^+}  + \ket{\Psi^-} )
$$
$$
\ket{VH}  =  \frac{1}{\sqrt{ 2 }} (\ket{\Psi^+}  -\ket{\Psi^-} )
$$
$$
\ket{VV}  =  \frac{1}{\sqrt{ 2 }} (\ket{\Phi^+}  - \ket{\Phi^-} )
$$
we get that we can rewrite each term in $\ket{\Psi}_{DABC}$, grouping by the DC photon:
- $\ket{VH}_{AB}$ is paired with $\ket{HH}_{DC}$
- $\ket{VV}_{AB}$ is paired with $\ket{HV}_{DC}$
- $\ket{HH}_{AB}$ is paired with $\ket{VH}_{DC}$
- $\ket{HV}_{AB}$ is paired with $\ket{VV}_{DC}$
Now let's substitute and collect terms by Bell state on AB. 
$$
\ket{\Psi} _{DABC} = \frac{1}{2} [\ket{\Psi^+}(\ket{HH}_{DC} + \ket{VV} _{DC} )  + \ket{\Psi^-}(\ket{HH}_{DC} - \ket{VV} _{DC} ) + \ket{\Phi^+}(-\ket{HV}_{DC} + \ket{VH} _{DC} ) + \ket{\Phi^-}(\ket{HV}_{DC} + \ket{VH} _{DC} )]
$$
Recognizing the Bell states of DC, we can rewrite it as
$$
\ket{\Psi} _{DABC} = \frac{1}{2} [\ket{\Psi^+}_{AB}\ket{\Phi^+} _{DC} + \ket{\Psi^-}_{AB}\ket{\Phi^-} _{DC} + \ket{\Phi^+}_{AB}\ket{\Psi^-} _{DC} + \ket{\Phi^-}_{AB}\ket{\Psi^+} _{DC}]
$$
Each outcome has probability 1/4, and D and C are now entangld regardless of which Bell state was measured on AB.

b)
We want to determine what unitary operation Bob should apply to photon C so that the final state of photons D and C becomes:
$$
\ket{\Psi^+} _{DC} = \frac{1}{\sqrt{ 2 }}(\ket{HV} _{DC}+\ket{VH} _{DC})
$$
From part a, we know that after a Bell-state measurement on AB, the state of DC becomes one of:
$$
\ket{\Psi^+} , \ket{\Psi^-} , \ket{\Phi^+} , \ket{\Phi^-}
$$
We now determine, for each case, what operation on photon C converts the state into $\ket{\Psi^+}$.
Case 1: DC in $\ket{\Psi^+}$
$$
\ket{\Psi^+} = \frac{1}{\sqrt{ 2 }}(\ket{HV} +\ket{VH} )
$$
This is already the desired state, so we just apply the identity matrix $\mathbf{I}$.
Case 2: DC in $\ket{\Psi^-}$
$$
\ket{\Psi^-} = \frac{1}{\sqrt{ 2 }}(\ket{HV} - \ket{VH} )
$$
Apply $\sigma_{z}$ on photon C:
$$
Z\ket{H}  = \ket{H} , Z\ket{V}  = -\ket{V}
$$
Then we get that
$$
\ket{\Psi^-} \to \frac{1}{\sqrt{ 2 }}(-\ket{HV} -\ket{VH} ) = - \ket{\Psi^+}
$$
Since overall phase is irrelevant, it must be that $\sigma_{z}$ is the correct unitary
Case 3: DC in $\ket{\Phi^+}$
$$
\ket{\Phi^+}  = \frac{1}{\sqrt{ 2 }}(\ket{HH} + \ket{VV}  )
$$
Apply $\sigma_{x}$ on photon C:
$$
X\ket{H}  = \ket{V} , X\ket{V} = \ket{H}
$$
Then we get that
$$
\ket{\Phi^+}  \to \frac{1}{\sqrt{ 2 }}(\ket{HV}  + \ket{VH} )
$$
Case 4: DC in $\ket{\Phi^-}$
$$
\ket{\Phi^-}  = \frac{1}{\sqrt{ 2 }}(\ket{HH} - \ket{VV}  )
$$
We apply $i\sigma_{y}$
$$
i\sigma_{y}\ket{H}  = \ket{V} , i\sigma_{y}\ket{V}  = -\ket{H} 
$$
Then we get that
$$
\ket{\Phi^-}  \to \frac{1}{\sqrt{ 2 }}(\ket{HV} + \ket{VH} )
$$

# 2. Bell Experiment with Other States
We consider the entangled state
$$
\ket{\Phi^+}  = \frac{1}{\sqrt{ 2 }}(\ket{HH}+\ket{VV}  )
$$
Now we define a polarization measurement at some angle $\theta$:
$$
\ket{+\theta} = \cos \theta \ket{H} +\sin \theta \ket{V}
$$
$$
\ket{-\theta} =-\sin \theta \ket{H} +\cos \theta \ket{V}
$$
Compute the probability that Alice measure + at angle $a$, and Bob measures + at angle $b$
$$
P_{++}(a,b)= |\braket{+a,+b|\Phi^+}|^{2}
$$
Expand the inner product
$$
\braket{+a|H}=\cos a, \braket{+a|V}=\sin a, \braket{+b|H}=\cos b, \braket{+b|V}=\sin b
$$
Then:
$$
\braket{+a, +b|HH} =\cos a\cos b
$$
$$
\braket{+a,+b|VV} =\sin a\sin b
$$
So:
$$
\braket{+a, +b|\Phi^+} = \frac{1}{\sqrt{ 2 }}(\cos a\cos b+\sin a\sin b)
$$
Then use the trig identity $\cos a\cos b+\sin a\sin b = \cos(a-b)$
$$
\braket{+a, +b|\Phi^+} = \frac{1}{\sqrt{ 2 }}\cos(a-b)
$$
Therefore
$$
P_{++}(a,b) = \frac{1}{2}\cos ^{2}(a-b)
$$
Similarly,
$$
P_{--}(a,b) = \frac{1}{2}\cos ^{2}(a-b)
$$
$$
P_{+-}(a,b) = \frac{1}{2} \sin ^{2}(a-b)
$$
$$
P_{-+}(a,b)=\frac{1}{2}\sin ^{2}(a-b)
$$
Now the correlation function is
$$
E(a,b) = (+1)(+1)P_{++}+(-1)(-1)P_{--}+(+1)(-1)P_{+-}+(-1)(+1)P_{-+}
$$
$$
= P_{++} + P_{--} - P_{+-} - P_{-+}
$$
Substitute:
$$
E(a,b) = \cos ^{2}(a-b) -\sin ^{2}(a-b)
$$
$$
E(a,b) = \cos(2(a-b))
$$
$$
S = E(a,b) -E(a,b') + E(a',b) +E(a',b')
$$
the allowed range $\left[ 0, \frac{\pi}{4} \right]$ limits us to have the maximum $S$ at $a=0, a'=\frac{\pi}{4},b=0,b'=\frac{\pi}{4}$. Then:
$$
S = \cos(0) - \cos\left( -\frac{\pi}{2} \right) + \cos\left( \frac{\pi}{2} \right) + \cos(0) = 1 - 0 +0 + 1 = 2
$$
Which is exactly at the classical bound. The issue is that the angle restriction given by the question means that the maximum difference is $\frac{\pi}{4}$, and cos doesnt go negative in the range $\left[ 0, \frac{\pi}{2} \right]$ we cant get the cancellation pattern needed. The CHSH inequality is not violated.

Re-derive the quantum-mechanical prediction for the Bell-CHSH parameter (and determine whether/when the CHSH inequality is violated) for entangled state other than $\ket{\Psi^-}$:
$$
\ket{\Phi^+} = \frac{1}{\sqrt{ 2 }}(\ket{HH}+\ket{VV}  ), \, \phi \in \left[ 0, \frac{\pi}{4} \right]
$$
