# Barn-Pole Paradox
A classic thought experiment with a surprisingly satisfying resolution. 
Consider a pole of proper length $L_{0}$ moving with velocity $v$ through a barn shorter than the pole in its rest frame.
Special relativity tells us that the moving pole will undergo length contraction
$$
L = \frac{L_{0}}{\gamma}, \space \gamma = \frac{1}{\sqrt{ 1 - \frac{v^{2}}{c^{2}} }}
$$
And if $v$ is large enough,
$$
L < L_{\text{barn}}
$$
So in barn frame, we get that the pole can fit. However, in pole's frame the barn is contracted and it definitely does not fit.
# Setup
Proper length of pole
$$
L_{0}
$$
Proper length of barn
$$
B_{0}
$$
with condition
$$
L_{0} > B_{0}
$$
# Barn Frame
Pole moves at velocity $v$, then by length contraction
$$
L = \frac{L_{0}}{\gamma}
$$
and if
$$
\frac{L_{0}}{\gamma} < B_{0}
$$
Both barn doors can close simultaneously, and the pole fits.
# Pole Frame
Now in this frame the barn moves instead. The barn undergoes length contraction
$$
B = \frac{B_{0}}{\gamma}
$$
and since $L_{0}>B_{0}$
$$
L_{0} > \frac{B_{0}}{\gamma}
$$
The pole does not fit, we reach a contradiction.
# Resolution
Here we arrive at one of the key concepts of relativity, which is the fact that "Simultaneity is relative". Events simultaneous in one frame are not simultaneous in another. We can see this fact from the Lorentz transformation
$$
t' = \gamma\left( t - \frac{vx}{c^{2}} \right)
$$
if two events are simultaneous $\Delta t = 0$. Then,
$$
\Delta t' = - \frac{\gamma (v\Delta x)}{c^{2}} \neq 0
$$
it's not simultaneous in another. In barn frame the doors close at the same time, but in pole frame the front door closes first, followed by the back door later.