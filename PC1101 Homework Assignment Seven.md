# 1. Accelerating Frame and Rindler Coordinates
$$
\begin{align}
t &= \left( \frac{c}{g} + \frac{x'}{c} \right)\sinh\left( \frac{gt'}{c} \right)  \\
x &= c \left( \frac{c}{g} + \frac{x'}{c} \right) \cosh\left( \frac{gt'}{c} \right) - \frac{c^{2}}{g} \\
y = y' \\
z = z',
\end{align}
$$
a) Let's start by computing the differentials. Let $\rho \equiv \frac{c}{g} + \frac{x'}{c}$ for brevity, so:
$$
dt = \frac{g}{c}\rho \cosh\left( \frac{gt'}{c} \right)dt' + \frac{1}{c} \sinh\left( \frac{gt'}{c} \right)dx'
$$
$$
dx = g\rho \sinh\left( \frac{gt'}{c} \right)dt' + \cosh\left( \frac{gt'}{c} \right)dx'
$$
$$
dy = dy', \space dz = dz'
$$
The Minkowski line element is $ds^{2} = -c^{2}dt^{2} + dx^{2} + dy^{2} + dz^{2}$. This quantity is invariant hence we can try substituting:
$$
ds^{2} = -c^{2}\left( \frac{g^{2}}{c^{2}}\rho^{2}\cosh ^{2}\left( \frac{gt'}{c} \right)dt'^{2}  + 2 \frac{g}{c^{2}}\rho \sinh\left( \frac{gt'}{c} \right)\cosh\left( \frac{gt'}{c} \right)dx'dt' + \frac{1}{c^{2}}\sinh ^{2}\left( \frac{gt'}{c} \right)dx'^{2}\right) 
$$
$$
+ \left( g^{2}\rho^{2}\sinh ^{2}\left( \frac{gt'}{c} \right)dt' + 2g\rho \sinh\left( \frac{gt'}{c} \right)\cosh\left( \frac{gt'}{c} \right)dx'dt' + \cosh ^{2}\left( \frac{gt'}{c} \right)dx'^{2} \right) + dy'^{2} + dz'^{2}
$$
Using $\cosh ^{2}-\sinh ^{2} = 1$,
$$
ds^{2} = -g^{2}\rho^{2}dt'^{2} + dx'^{2} + dy'^{2} + dz'^{2}
$$
$$
ds^{2} = - \left( 1 + \frac{gx'}{c^{2}} \right)^{2} c^{2}dt'^{2} + dx'^{2} +dy'^{2} + dz'^{2}
$$
b) Using $\sinh\left( \frac{gt'}{c} \right) \approx \frac{gt'}{c}$ and $\cosh\left( \frac{gt'}{c} \right) \approx 1$. We expand $x$ to second order in $t'$:
$$
x \approx \left( \frac{c^{2}}{g} + x' \right) \left( 1 + \frac{1}{2} \frac{g^{2}t^{2}}{c^{2}} \right) - \frac{c^{2}}{g} = x' + \frac{1}{2}gt'^{2} \left( 1 + \frac{gx'}{c^{2}} \right)
$$
To leading (Newtonian) order: $x \approx x' + \frac{1}{2}gt'^{2}$, i.e. uniform acceleration $\ddot{x} = g$ from rest.

c) For a clock at rest at position $x'$ in the prime frame, $dx'=dy'=dz'=0$, so proper time is:
$$
d\tau = \sqrt{ -\frac{ds^{2}}{c^{2}} } = \left( 1 + \frac{gx'}{c^{2}} \right)dt'
$$
Thus:
- Clock at $x'=0$: $d\tau_{0} = dt'$
- Clock at $x' = h$: $d\tau_{h} = (1 + \frac{gh}{c^{2}})dt'$
The ratio is:
$$
\frac{d\tau_{h}}{d\tau_{0}} = 1 + \frac{gh}{c^{2}}
$$

d) At a fixed $t'$, the spatial metric is $d'^{2} = dx'^{2} + dy'^{2} + dz'^{2}$. So the distance between $x'=0$ and $x'=h$ is $\int^h_{0}dx'=h$, which is a constant, so its rigid motion as its independent from time.

e) From part (c), proper time at $x'$ runs at rate $\left( 1 + \frac{gx'}{c^{2}} \right)$ relative to coordinate time $t'$. The observer at $x'=0$ is defined to have proper acceleration $g$. Any observer at $x'$ has the same coordinate motion scaled by the factor $\left( 1 + \frac{gx'}{c^{2}} \right)$, visible from the transformation since $\rho = \frac{c}{g} + \frac{x'}{c}$ just rescales everything. Proper acceleration then scales inversely, giving
$$
\frac{g}{1 + \frac{gx'}{c^{2}}}
$$
# 2. Hafele-Keating Experiment
a) Work in an inertial frame centred on Earth's centre. A surface clock at radius $R_{\oplus}$ moves with speed $V_{\oplus}$ due to Earth's rotation. A flying clock is at altitude $h(t)$ and has ground speed $V_{g}(t)$ relative to the surface, so its speed in the inertial frame is $V_{g}+V_{\oplus}$ (for eastward flight).

The metric outside Earth (weak field, slow motion) gives proper time:
$$
d\tau \approx \left( 1 + \frac{\phi}{c^{2}} - \frac{v^{2}}{2c^{2}} \right)dt
$$
where $\phi = - \frac{GM}{r}$ is the gravitational potential and $v$ is the speed in the inertial frame. Taking $\phi \approx -\frac{GM}{R_{\oplus}} + gh$ with $g = \frac{GM}{R_{\oplus}^{2}}$

Flying clock:
$$
d\tau_{fly} \approx \left( 1 - \frac{GM}{R_{\oplus}c^{2}} + \frac{gh}{c^{2}} - \frac{(V_{g}+V_{\oplus})^{2}}{2c^{2}} \right)dt
$$
Surface clock:
$$
d\tau_{surf} \approx \left( 1 - \frac{GM}{R_{\oplus}c^{2}} - \frac{V_{\oplus}^{2}}{2c^{2}} \right)dt
$$
The difference $\Delta \tau = \int(d\tau_{fly}-d\tau_{surf})$:
$$
\Delta \tau = \frac{1}{c^{2}} \int dt \left[ gh(t) - \frac{1}{2} V_{g}(t)(V_{g}(t) + 2V_{\oplus}) \right]
$$
b) Use typical values: $h\approx 10 km$, $V_{g} \approx 800 \frac{km}{h} \approx 222 \frac{m}{s}$, $g \approx 9.8 \frac{m}{s^{2}}$, $V_{\oplus} \approx 465 \frac{m}{s}$, and a circumnavigation takes $T \approx \frac{40000}{800} \approx 50 hr = 1.8 \times 10^5 s$, with 40000 the circumference of the earth.

Gravitational term (same for both directions):
$$
\frac{ghT}{c^{2}} \approx +204 ns
$$
Kinematic term:
$$
-\frac{T}{2c^{2}}V_{g}(V_{g} + 2V_{\oplus})
$$
- Eastward $V_{g} = + 222$,  $V_{\oplus}$: $\approx -270 ns$
- Westward $V_{g}=-222$, $V_{\oplus}$: $\approx +166 ns$
Then we have a total $\Delta \tau$ of -66 ns for eastward, and 370 ns for west ward.