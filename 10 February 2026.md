# Newton's 1st law
A free particle moves on a straight line at constant speed
$$
\frac{d^{2}r}{dt^{2}} = 0
$$
Inertial frames could be defines as Cartesian reference frames for which Newton's 1st law holds in the above form
Caution: Not every Cartesian coordinate system is an inertial frame

## Newtonian Space is Flat
Newtonian mechanics assumes a flat, Euclidean geometry for space, specified in Cartesian coordinates (x,y,z) by the line element:
$$
ds^{2} = dx^{2} + dy^{2} + dz^{2}
$$
and a separate, single "absolute", "universal" notion of time for all inertial observers:
$$
t' = t
$$
In particular, two events that are simultaneous, they occur at the same time, in one inertial frame are simultaneous in every other inertial frame.

# Coordinate Transformation
There are many inertial frames.
	Displacements
	Rotations
	Uniform motions
	Combinations of above three

## Galilean Transformation
Combination of uniform motion in spatial coordinate system and the assumption of absolute time
$$
x' = x-vt, \space y'=y, \space z'=z, \space t'=t
$$

## Principle of Relativity
Equation of motion for free particles is invariant under Galilean transformation
$$
\frac{d^{2}r'}{dt^{2}} = 0
$$
For particles with forces acting on it, newton's 2nd law remains the same:
$$
\mathbf{F}' = m \mathbf{a}'
$$
Principle of Relativity:
	Identical experiments carried out in different inertial frames give identical results
$\Rightarrow$ Speed of light is the same $c$ in different reference frames.
Simultaneity is relative.

## Simultaneity - Rest Frame
Observer $O$ is midway between $A$ and $B$.
$A$ and $B$ each emit light signals toward $O$.
$O$ receives the signals simultaneously.

## Simultaneity - Moving Frame
Observer $O$ is midway between $A$ and $B$.
$A$ and $B$ each emit light signals toward $O$.
$O$ receives the signals simultaneously.
Signal $A$ is emitted earlier.
Two events simultaneous in one inertial frame are not simultaneous in one moving wrt the first if the velocity of light is the same in both.

## Spacetime
There is generally a different notion of simultaneity and time for each inertial frame.
The correct geometric arena for physics is a 4D unification of space and time -spacetime.
Inertial frames are spanned by 4 Cartesian coordinates: $(t,x,y,z)$.
A different inertial frame has a different set of 4 coordinates: $(t',x',y',z')$.

## Model Clock in Rest Frame
Consider two parallel mirrors separated by a distance $D$ at rest in an inertial frame (Sally) in which events are described by coordinates $(t_{0},x_{0},y_{0},z_{0})$.
A light signal bounces back and forth between the mirror.s
A clock measures the time interval $\Delta t_{0}$ between event 1 of the departure of the light ray and event 2 of its return to the same point in space.

## Uniformly Moving Frame
Sam is moving with speed $v$ wrt Sally along the negative $x_{0}$-direction parallel to the mirrors.
In this inertial frame the mirrors are moving with speed $v$ along the positive x-direction.
The coordinate intervals between Events 1 and 2 in this frame are
$$
\Delta t = \frac{2}{c}\sqrt{ D^{2} + \left( \frac{1}{2}\Delta x \right)^{2} }, \space \Delta x = v\Delta t, \space \Delta y = \Delta z=0
$$

# Invariance
Note: the transverse distances are the same in both inertial frames.
Observe that
$$
-(c\Delta t)^{2} + (\Delta x)^{2} = -4D^{2} = -(c\Delta t_{0})^{2}
$$
Or
$$
-(cdt)^{2} + (dx)^{2} + (dy)^{2} + (dz)^{2} = -(cdt_{0})^{2} + (dx_{0})^{2}+(dy_{0})^{2} + (dz_{0})^{2}
$$
$$
ds^{2}=ds_{0}^{2}
$$
An invariance between these two inertial frames

## Minkowski Space
It turns out that the quantity
$$
ds^{2} = -(cdt)^{2} + (dx)^{2} + (dy)^{2} + (dz)^{2}
$$
is invariant under the change in inertial frames
	Displacements
	Lorentz boosts
	Rotations
	Combinations of the above
it is also non-Euclidean

The views of space and time which I wish to lay before you have sprung from the soil of experimental physics, and therein lies their strength. They are radical. Henceforth, space by itself, and time by itself, are doomed to fade away into mere shadows, and only a kind of union of the two will preserve an independent reality. (Minkowski, 1909)

## 2D Euclidean Space
Finite interval in 2D Euclidean space:
$$
\Delta s^{2} = \Delta x^{2} + \Delta y^{2}
$$
Infinitesimal interval:
$$
ds^{2}=dx^{2}+dy^{2}
$$
It is invariant under
	Translation
	Rotation
	Combination of the two transformations

### Translation
For example, a translation in $x$-direction:
$$
x'=x-d, \space y'=y
$$
A general 2D translation:
$$
dx'=dx, \space dy' =dy
$$
Invariant interval:

### Rotation
Rotation by angle $\phi$:
$$
x'=x\cos \phi+y\sin \phi, \space y' = -x\sin \phi+y\cos \phi
$$
$$
ds'^{2} = dx'^{2}+dy'^{2} = dx^{2}+dy^{2}=ds^{2}
$$

## 2D Minkowski Space
Infinitesimal interval in 1+1D Minkowski spacetime:
$$
ds^{2}=-c^{2}dt^{2}+dx^{2}
$$
It is invariant under
	Translation
	Rotation
	Combination of the two

### Lorentz Boost
Lorentz boost by $\theta$:
	$ct' = ct\cosh \theta -x\sinh \theta$
	$x'=-ct\sinh \theta + x\cosh \theta$
Lorentz invariance
$$
ds'^{2}=ds^{2}
$$
Velocity of $S'$ relative to $S$:
$$
v = c\tanh \theta
$$

