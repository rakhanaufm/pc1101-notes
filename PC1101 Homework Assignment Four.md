Muhammad Rakha Naufal Maulana A0330820U
# 1. Sellmeier's Equation
a) Using the Taylor expansion, and considering only one resonance, we have that for $(\frac{\omega}{\omega_{0}})^{2} \ll 1$,
$$
n^{2}_{SE}(\omega) \approx 1 + B \left(  1 + \frac{\omega^{2}}{\omega_{0}^{2}} \right)
$$
b) After squaring and using the Taylor expansion again, we get (retaining the first and second term because the third term is negligibly small)
$$
n^{2}_{toy}(\omega) \approx 1 + \frac{2c\gamma}{a\omega_{0}^{2}} \left( 1 + \frac{\omega^{2}}{\omega_{0}^{2}} \right)
$$
Which means that for the two models to be consistent,
$$
B = \frac{2c\gamma}{a\omega_{0}^{2}}
$$
c) We can divide the summation term by $\lambda^{2}$ to get,
$$
n^{2}_{SE}(\lambda) = 1 + \sum_{i} \frac{B_{i}}{1 - \frac{C_{i}}{\lambda^{2}}}
$$
This is exactly the same as Eq. (1) if we have the condition 
$$
\frac{C_{i}}{\lambda^{2}} = \frac{\omega^{2}}{\omega_{i}^{2}}
$$
or,
$$
C_{i} = \left(\frac{\omega \lambda}{\omega_{i}}\right)^{2} = \left(\frac{2\pi c}{\omega_{i}}\right)^{2}
$$
# 2. Discovering Evanescent Waves
a) From Snell's Law, we have
$$
n_{i}\sin \theta_{i} = n_{t} \sin \theta_{t}
$$
Rearranging gives us,
$$
\sin \theta_{t} = \frac{n_{i}}{n_{t}}\sin \theta_{i}
$$
and,
$$
\cos \theta_{t} = \sqrt{ 1 - \left( \frac{n_{i}}{n_{t}}\sin \theta_{i} \right)^{2} }
$$
b) Plugging this back into the expression $e^{i(\mathbf{k}_{t}\cdot \mathbf{r} - \omega t)}$ gives,
$$
e^{i(k_{t,x}x + k_{t,y}y - \omega t)} = e^{i \cdot \pm ik_{t} \sqrt{ (n_{i}\sin \theta_{i}/n_{t})^{2} - 1 }y} e^{i(k_{t}\sin \theta_{i}x -\omega t)} = e^{-y/d}e^{i(k_{t}\sin \theta_{i}x - \omega t)}
$$
with 
$$
\frac{1}{d} = k_{t}\sqrt{\left( \frac{n_{i}}{n_{t}}\sin \theta_{i} \right)^{2}-1  }
$$
$$
d = \frac{1}{k_{t}\sqrt{\left( \frac{n_{i}}{n_{t}}\sin \theta_{i} \right)^{2}-1   }} = \frac{c}{\omega n_{t}} \frac{1}{\sqrt{ \left( \frac{n_{i}}{n_{t}}\sin \theta_{i} \right)^{2}-1  }}
$$
The other solution $e^{+y/d}$ is omitted because it doesn't make any physical sense, as the wave would be amplified.
c) If the low index layer thickness is small $l \ll d$, the evanescent field does not decay significantly before reaching the second interface. Leading to some of the light being transmitted instead of fully reflected
