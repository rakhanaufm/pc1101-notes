Muhammad Rakha Naufal Maulana A0330820U
# 1. The Barn-Pole Paradox
The resolution is that simultaneity is relative. From the Barn's frame, the doors seem to close simultaneously. However, in runner's frame it seems that the front door closes first, and then the rear door closes. I have plotted the worldline for this "paradox" below.
![[Light.png]]
As you can see, the two striped blue and yellow lines intersection appear earlier according to the dotted black line. Whereas the solid blue and yellow lines intersection appear much later. Proving that indeed, the front door closes first than the rear.
# 2. Simple Accelerated Particle
a)
No, as we can see even as $t \to \infty$, its speed is capped at $c$
$$
\frac{dx}{dt} \approx \frac{gt}{\sqrt{ g^{2}t^{2} }}c  = c
$$
b)
We first compute,
$$
\gamma = \frac{1}{\sqrt{ 1 - \frac{v^{2}}{c^{2}} }}
$$
with
$$
v^{2} = \frac{g^{2}t^{2}}{1 + \frac{g^{2}t^{2}}{c^{2}}}
$$
$$
\frac{v^{2}}{c^{2}} = \frac{\frac{g^{2}t^{2}}{c^{2}}}{1 + \frac{g^{2}t^{2}}{c^{2}}}
$$
$$
1 - \frac{v^{2}}{c^{2}} = \frac{1}{1 + \frac{g^{2}t^{2}}{c^{2}}}
$$
thus,
$$
\gamma = \sqrt{ 1 + \frac{g^{2}t^{2}}{c^{2}} }
$$
Four-velocity is
$$
U^{0} = \gamma c, U^x = \gamma v
$$
substitute $v$
$$
U^x = \sqrt{ 1 + \frac{g^{2}t^{2}}{c^{2}} } \frac{gt}{\sqrt{ 1 + \frac{g^{2}t^{2}}{c^{2}} }}
$$
$$
U^x = gt
$$ 
In the end,
$$
U^\mu = \left( c \sqrt{ 1 + \frac{g^{2}t^{2}}{c^{2}} }, gt, 0 , 0\right)
$$
c)
Proper time is,
$$
d\tau = \frac{dt}{\gamma} = \frac{dt}{\sqrt{ 1 + \frac{g^{2}t^{2}}{c^{2}} }}
$$
Integrating,
$$
\tau = \frac{c}{g}\sinh^{-1} \left( \frac{gt}{c} \right)
$$
using $t=0, \tau = 0$.
Now to get $t$, we have to take the inverse
$$
t(\tau) = \frac{c}{g}\sinh\left( \frac{g\tau}{c} \right)
$$
Let's now find $x(t)$
$$
\frac{dx}{dt} = \frac{gt}{\sqrt{ 1 + \frac{g^{2}t^{2}}{c^{2}} }}
$$
integrating,
$$
x = \frac{c^{2}}{g} \left( \sqrt{ 1 + \frac{g^{2}t^{2}}{c^{2}} } -1 \right)
$$
Notice that,
$$
\sqrt{ 1+\sinh ^{2}u } = \cosh u
$$
we get
$$
x(\tau) = \frac{c^{2}}{g} \left[ \cosh(\frac{g\tau}{c}) -1 \right]
$$
We then have,
$$
t(\tau) = \frac{c}{g}\sinh\left( \frac{g\tau}{c} \right)
$$
$$
x(\tau) = \frac{c^{2}}{g} \left[\cosh\left( \frac{g\tau}{c} \right) - 1\right]
$$
d)
To get the worldline equation, we must first eliminate $\tau$
$$
x + \frac{c^{2}}{g} = \frac{c^{2}}{g}\cosh\left( \frac{g\tau}{c} \right)
$$
$$
ct = \frac{c^{2}}{g}\sinh\left( \frac{g\tau}{c} \right)
$$
Then use the hyperbolic identity
$$
\cosh ^{2}-\sinh ^{2} = 1
$$
to get,
$$
\left( x + \frac{c^{2}}{g} \right)^{2} - (ct)^{2} = \left( \frac{c^{2}}{g} \right)^{2}
$$
Plotting this into desmos, using $c=1,g=1$ and using $y$-axis as $t$-axis
![[Pasted image 20260306131605.png]]
we get a hyperbole. IIRC this is called Rindler coordinates, which are used for trajectories of objects with constant proper acceleration.

e)
Using the definition of the four-acceleration,
$$
A^\mu = \frac{dU^\mu}{d\tau}
$$
thus, for four-velocity with components
$$
U^0 = c\cosh\left( \frac{g\tau}{c} \right), U^x = c\sinh\left( \frac{g\tau}{c} \right)
$$
the four-acceleration is thus,
$$
A^0 = g\sinh\left( \frac{g\tau}{c} \right), A^x = g\cosh\left( \frac{g\tau}{c} \right)
$$
For our four-force, we get,
$$
F^\mu = mA^\mu
$$
$$
F^\mu = \left( mg\sinh\left( \frac{g\tau}{c} \right), mg\cosh\left( \frac{g\tau}{c} \right), 0 , 0 \right)
$$
Now, checking our three force, we have for the momentum
$$
p = \gamma mv
$$
however, notice that
$$
\gamma v = gt
$$
thus,
$$
p= mgt
$$
$$
F = \frac{dp}{dt} = mg
$$
which shows that the three force is constant.