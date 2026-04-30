# 4-Vectors
Specifying the components of a four-vector and the basis four-vectors is equivalent to specifying the four-vector itself
Four-vectors can be added, substracted, and multiplied by numbers according to the usual rules for vectors
The components of a four
# Applications of Special Relativity
## Length Contraction
Consider a rod whose length is $L_{\star}$ when measured in its own rest frame.
$$
x' = \gamma(x-vt), t' = \gamma\left( t- \frac{vx}{c^{2}} \right)
$$
$$
\Delta x' = \gamma(\Delta x -v\Delta t), \Delta t' = \gamma\left( \Delta t - \frac{v}{c^{2}}\Delta x \right)
$$
$$
\Delta t'=0, \Delta x' = L, \Delta t \neq 0 , \Delta x = L_{\star}
$$
$$
\begin{cases}
L &= \gamma(L_{\star}-v \Delta t) \\
0 &= \gamma\left( \Delta t - \frac{v}{c^{2}}L_{\star} \right) \Rightarrow \Delta t = \frac{v}{c^{2}}L_{\star} 
\end{cases}
$$
$$
L = \frac{L_{\star}}{\gamma}
$$
## Time Dilation vs. Length Contraction
Stationary rod measured by a moving observer
$$
L = v\Delta t = v\Delta \tau
$$
Same events measured by a rest observer
$$
L_{\star} = v\Delta t'
$$
By time dilation
$$
\Delta \tau = \Delta t' \sqrt{ 1 - \frac{v^{2}}{c^{2}} }
$$
We get length contraction
$$
L =L_{\star} \sqrt{ 1 - \frac{v^{2}}{c^{2}} }
$$
They are consistent!
## Time Dilation & the Twin Paradox
Time dilation: $d\tau = \sqrt{ 1 - \frac{v^{2}(t)}{c^{2}} }dt < dt$
$$
\tau_{AB} = \int^B_{A} d\tau = \int^{t_{B}}_{t_{A}}dt \sqrt{ 1 - \frac{v^{2}(t)}{c^{2}} } < t_{B} - t_{A}
$$
## Twin Paradox Example
Astronaut Alice takes a space trip at a speed of $\beta = 0.65$ to a space station located 3.25 light-years from Earth and back starting on the 20th birthday while her twin brother Bob stays at home on Earth.
The round trip distance is 6.5 light-years, so from Bob's point of view on Earth, Alice's trip takes
$$
\frac{6.50}{0.65} = 10 \space \text{years}
$$
So when Alice returns, Bob is 20 + 10 = 30 years old
## Length Contraction
The gamma parameter for Alice is
$$
\gamma = \frac{1}{\sqrt{ 1- 0.65^{2} }} = 1.315
$$
From Alice's point of view, she travels a length contracted distance
$$
\frac{6.5}{1.315} = 4.942
$$
From Alice's point of view, the trip takes
$$
\frac{4.942}{0.65} = 7.6 \space \text{years}
$$
When she returns, Alice is 20 + 7.6 = 27.6 years old
## The Paradox
Now let's look at Bob from Alice's point of view
Whe seems to be sitting still and Bob is moving with speed $\beta=0.65$
Alice ages 7.6 years during her trip, but Bob was moving with $\beta = 0.65$ $(\gamma \approx 1.316)$ so his clock was running more slowly and he should have aged
$$
\frac{7.6}{1.316} = 5.8 \space \text{years}
$$
So when Alice returned to Earth, she would be 27.6 years old and Bob would be 25.8 years old
Both twins can't be younger than the other!
Which of these two views is right?
## Resolution of the Twin Paradox
The resolution of the twin paradox comes when we realize that Bob remains in an inertial frame on Earth while Alice lives in two different inertial frames during her trip
	An outbound leg where she moves away from Earth and towards the space station
	An inbound leg where she moves back from the space station towards Earth
	The symmetry between the twins is broken!
We can analyze the path of the two twins by counting "Happy Birthday" signals they received from each other
## Twin Paradox - Other Arguments
Sometimes you hear that the lack of aging for the flying twin occurs when the flying twin accelerates to turn around and come back and the effects of general relativity take over
We showed that the twin paradox can be resolved using the special theory of relativity only
We did have to invoke acceleration to turn the flying twin around, but we can postulate various scenatios to minimize the contributions from this acceleration
The effects of general relativity are not required to explain the paradox
## Addition of Velocities in Newtonian Physics
Galilean Transformation
$$
\begin{cases}
x =& x' + vt' \\
t =& t'
\end{cases}
\Rightarrow \begin{cases}
dx = dx' + vdt' \\
dt = dt'
\end{cases}
\Rightarrow
\frac{dx}{dt} = \frac{dx'}{dt'} + v
$$
Let $v_{1} = \frac{dx'}{dt'}, v_{2} =v, v_{1+2} = \frac{dx}{dt}$
$$
v_{1+2} = v_{1} + v_{2}
$$
## Addition of Velocities in SR
Lorentz transformation
$$
\begin{cases}
t = \gamma\left( t' - \frac{vx'}{c^{2}} \right) \\
x = \gamma(x' - vt') 
\end{cases}
$$
Differentiating, we get
$$
\begin{cases}
dt = \gamma\left( dt' - \frac{vdx'}{c^{2}} \right) \\
dx = \gamma(dx' - vdt')
\end{cases}
$$
taking $\frac{dx}{dt}$, we get
$$
\frac{dx}{dt} = \frac{\left( dt' - \frac{vdx'}{c^{2}} \right)}{dx' - vdt'} = \frac{\left( 1 - \frac{vdx'}{dt'c^{2}} \right)}{\frac{dx'}{dt'} - v}
$$
Rearranging for $\frac{dx'}{dt'}$ and using $v_{1+2} = \frac{dx'}{dt'}$ and $u = \frac{dx}{dt}$, we get
$$
v_{1+2} = \frac{u + v}{1 + \frac{uv}{c^{2}}}
$$
## Why $c+c=c$?
Relativistic addition for the case when the two objects move in the opposite direction:
$$
v_{1+2} = \frac{v_{1} + v_{2}}{1 + \frac{v_{1}v_{2}}{c^{2}}}
$$
For speed small compared to $c$, we can neglect $\frac{v_{1}v_{2}}{c^{2}}$ compared to 1, and we get back our Galilean result.
## Example
Relativistic addition for the case when the two objects move in the same direction:
$$
v_{1-2} = \frac{v_{1}-v_{2}}{1- \frac{v_{1}v_{2}}{c^{2}}}
$$
Example: The shuttlecraft Sacagawea is approaching the starship Voyager. With respect to the surrounding stars, the speeds of the spacecraft are
	$v_{s}$ = 0.830c
	$v_{v}$ = 0.750c in the same direction
What is the speed of Voyager as observed from Sacagawea?
$$
v_{v-s} = \frac{v_{v}-v_{s}}{1- \frac{v_{v}v_{s}}{c^{2}}}
$$

$$
E^{2} = \gamma^{2}m^{2}c^4
$$
$$
\gamma^{2} = \frac{1}{1 - \frac{v^{2}}{c^{2}}} = \frac{c^{2}}{c^{2}-v^{2}} = \frac{\frac{E}{\gamma m}}{\frac{E}{\gamma m} - \frac{p^{2}}{\gamma^{2}m^{2}}} \Rightarrow c^{2}(\gamma^{2}-1) = v^{2}
$$

$$
\frac{p}{\gamma m} = v
$$
$$
p^{2} = \gamma^{2}m^{2}v^{2}
$$

$$
E^{2} = p^{2} \frac{c^4}{v^{2}} = p^{2}c^{2} + m^{2}c^4
$$
$$
p^{2} = \frac{m^{2}v^{2}}{1- \frac{v^{2}}{c^{2}}}
$$
$$
p^{2} - \frac{p^{2}v^{2}}{c^{2}} = m^{2}v^{2}
$$
$$
v^{2} = \frac{p^{2}}{\frac{p^{2}}{c^{2}}+ m^{2}} = \frac{p^{2}c^{2}}{p^{2} + m^{2}c^{2}}
$$
$$
\gamma^{2} = \frac{1}{1- \frac{\frac{p^{2}}{\frac{p^{2}}{c^{2}}+m^{2}}}{c^{2}}} = 1 + \frac{p^{2}}{m^{2}c^{2}}
$$
$$
E^{2} = \left( 1+ \frac{p^{2}}{m^{2}c^{2}} \right)m^{2}c^4 = m^{2}c^4 + p^{2}c^{2}
$$
$$
E = \sqrt{ p^{2}c^{2} + m^{2}c^4 }
$$
