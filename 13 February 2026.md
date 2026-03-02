# Lorentz Boosts in terms of the relative velocity
$$
v=c\tanh \theta
$$
$$
\frac{v^{2}}{c^{2}}=\frac{\sinh^{2}\theta}{\cosh ^{2}\theta} \Rightarrow 1 - \frac{v^{2}}{c^{2}} = 1 - \frac{\sinh ^{2}\theta}{\cosh ^{2}\theta} = \frac{1}{\cosh ^{2}\theta}
$$
$$
\Rightarrow \cosh \theta = \pm \frac{1}{\sqrt{ 1-\frac{v^{2}}{c^{2}} }} = \frac{1}{\sqrt{ 1-\frac{v^{2}}{c^{2}} }} \equiv \gamma
$$
$$
\sinh \theta = \tanh \theta \cosh \theta = \frac{v}{c}\gamma
$$
Relativistic factor: $\gamma \geq 1$

## Lorentz Boost (cont)
$$
t'= \gamma\left( t- \frac{vx}{c^{2}} \right), \space x' = \gamma(x-vt)
$$
$$
ct' = ct\cosh \theta - x \sinh \theta, \space x' = -ct \sinh \theta + x\cosh \theta
$$

## Relativity of Simultaneity
Consider 2 events $A$ and $B$, which are simultaneous for an observer in the $(ct',x')$ frame:
$$
t= \gamma \left( t' + \frac{v}{c^{2}}x' \right), \space \Delta t=\gamma\left( \Delta t' + \frac{v}{c^{2}}\Delta x' \right)
$$
$$
\Delta t'=0, \Delta t= \gamma\frac{ v}{c^{2}} \Delta x'
$$
$$
\Delta t_{AB} =\gamma \frac{v}{c^{2}} \Delta x_{AB}'
$$
# Light Cone
An event occurs at time $0$ at location $x_{0}$
A signal that announces this event in space and time can propagate no faster than the speed of light with a velocity: $-c\leq v \leq c$
The tan-colored triangle shows the region in space and time in which the event can be observed
This region is called the future light cone of the event


## Causality
The blue point located at time $t_{1}$ and position $x_{1}$ is able to receive a signal that the original event has happened
The green point located at time $t_{2}$ and position $x_{2}$ is not able to receive such a signal
This implies that the events represented by the red dot cannot possibly have caused the event represented by the green dot
The two events, red and green, cannot be causally connected, i.e., one event cannot cause the other

# More Light Cones
Usually light cones are shown with position on the horizontal axis and time on the vertical axis
Events in the past light cone can influence the events at the origin
Events at the origin can influence events in the future light cone
Why do we call these drawing light cones instead of light triangles?
It is more obvious when we use two spatial dimensions, $x$ and $y$, along with time, $t$
## Different Velocities
We scale the axes of the light cone so that they have the same units
Assume an object initially located at $x=0$ and $t=0$
Vector 1 shows an object that is not moving
Vector 2 shows an object moving in the positive $x$ direction
Vector 3 shows an object moving in the negative $x$ direction
Vector 4 shows an object moving with the speed of light in the positive $x$ direction
Vector 5 shows an object moving with the speed of light in the negative $x$ direction
# Spacetime Diagrams and Worldlines
A spacetime diagram is a plot of two (or more) of the coordinate axes of an inertial frame
A worldline is the trajectory of an object in space and time, or spacetime

## Timelike Separations
The points that are timelike separated from P lie inside the light cone:
$$
(\Delta s)^{2} = -(c\Delta t)^{2} +(\Delta x)^{2} + (\Delta y)^{2} + (\Delta z)^{2} <0
$$
$$
\left( \frac{\Delta x}{\Delta t} \right)^{2} + \left( \frac{\Delta y}{\Delta t} \right)^{2} + \left( \frac{\Delta z}{\Delta t} \right)^{2} = \bar{v}^{2} < c^{2}
$$

## Timelike Separations - Example
Example: When two points are at the same place but at different times
then
$$
(\Delta s)^{2} = -(c\Delta t)^{2} +(\Delta x)^{2} + (\Delta y)^{2} + (\Delta z)^{2} =-(c\Delta t)^{2} < 0
$$
A clock is a device that measures timelike distances $\Delta \tau$:
$$
(\Delta \tau)^{2} \equiv - \frac{1}{c^{2}}(\Delta s)^{2}
$$
$\tau$ is called the proper time, and it is invariant!
## Timelike World Lines
Particles with nonzero rest mass move along timelike world lines inside the light cone of any point along their trajectory.
Their velocity is always less than the speed of light at any point.
A clock carried along a timelike world line measures proper time $\tau$

# Model Clock Revisited
From geometry:
$$
L = \sqrt{ \left( \frac{1}{2}v\Delta t \right)^{2} + D^{2} }
$$
Substitute $D = \frac{1}{2}vt_{0}$
$$
\Delta t = \gamma \Delta t_{0}
$$
Eliminate $L$
$$
\Delta t = \frac{\Delta t_{0}}{\sqrt{ 1-\left( \frac{v}{c} \right)^{2} }} = \gamma\Delta t_{0}
$$
Time dilation:
$$
\Delta \tau \equiv \Delta t_{0} = \Delta t \sqrt{ 1-\left( \frac{v}{c} \right)^{2} }
$$
## Time Dilation
The rate at which time flows depends on how fast the observer moves!
$$
\Delta t = \frac{\Delta t_{0}}{\sqrt{ 1-\left( \frac{v}{c} \right)^{2} }} = \gamma t_{0}
$$
Note: this is not just the subjective perception of time, but the objective measurable length of time!
# Why Haven't We Noticed...
It is convenient to express speeds as fractions of $c$
Introduce $\beta$
$$
\beta = \frac{v}{c}
$$
Then we get for $\gamma$
$$
\gamma = \frac{1}{\sqrt{ 1- \beta^{2} }}
$$

### Example: Time Dilation in Muon Decay
Muons have a lifetime of $2.2 \mu s$ 
CERN experiment: muons produced with $\beta$ = 0.9994
$$
\gamma = 28.87
$$
Lifetime of these moving muons should be 28.87 times longer, 63.5 $\mu$s, than for those at rest.
During this time, the muons can move a distance
$$
x = v\tau = v\gamma \tau_{0} = 19 km
$$
Without time dilation, this distance would only be 660 m
-> Direct observation of time dilation!

# Spacelike Separations
Points that are spacelike separated from P lie outside the light cone

$$
(\Delta s)^{2} = -(c\Delta t)^{2} +(\Delta x)^{2} + (\Delta y)^{2} + (\Delta z)^{2} >0
$$
$$
\left( \frac{\Delta x}{\Delta t} \right)^{2} + \left( \frac{\Delta y}{\Delta t} \right)^{2} + \left( \frac{\Delta z}{\Delta t} \right)^{2} = \bar{v}^{2} > c^{2}
$$

## Spacelike Separations - Example
When two points are at the same time but at different places
Ruler is a device that measures spacelike distances.

# 3-Vectors in Euclidean Space
A three-vector $\vec{a}$ can be defined as a directed line segment in 3D Euclidean space.
In a particular coordinate system,
$$
\mathbf{a} = \sum_{i}a^i \mathbf{e}_{i} = a^x\mathbf{x} + a^y\mathbf{e}_{y} + a^z\mathbf{e}_{z}
$$
Specifically, position vector
$$
\mathbf{r} = x\mathbf{e}_{x} + y\mathbf{e}_{y} + z\mathbf{e}_{z}
$$
Scalar product of two three-vectors $\mathbf{a}$ and $\mathbf{b}$:
$$
\mathbf{a}\cdot \mathbf{b} = \sum_{i,j}(a^i\mathbf{e}_{i})\cdot(b^j\mathbf{e}_{j}) = \sum_{i,j} a^ib^j\mathbf{e}_{i}\cdot\mathbf{e}_{j} = \sum_{i,j}\delta_{ij}a^ib^j
$$
provided orthonormal basis:
$$
\mathbf{e}_{i}\cdot \mathbf{e}_{j} = \delta_{ij} = \begin{cases}
1,& i=j \\
0,& i\neq j
\end{cases}
$$
Scalar product has properties:
$$
\mathbf{a}\cdot \mathbf{b} = \mathbf{b}\cdot \mathbf{a}
$$
$$
\mathbf{a}\cdot(\mathbf{b}+\mathbf{c}) = \mathbf{a}\cdot \mathbf{b} + \mathbf{a}\cdot \mathbf{c}
$$
$$
(\alpha \mathbf{a})\cdot \mathbf{b} = \alpha(\mathbf{a}\cdot \mathbf{b})
$$
# 4-Vectors in Flat Spacetime
A four-vector $\mathbf{a}$ is defined as a directed line segment in four-dimensional flat spacetime.
In a particular inertial frame,
$$
a = a^te_{t} + a^xe_{x} + a^ye_{y} + a^ze_{z}
$$
or equivalently,
$$
\mathbf{a} = \sum^3_{\mu=0} a^\mu \mathbf{e}_{\mu}
$$
Einstein summation convention
$$
\mathbf{a} = a^\mu \mathbf{e}_{\mu}
$$
